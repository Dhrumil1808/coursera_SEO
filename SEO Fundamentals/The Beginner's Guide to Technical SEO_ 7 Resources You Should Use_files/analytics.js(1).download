(function(){
    //Don't do anything if embedded as an iframe
    jQuery.urlParam = function(name,url){
	if(!url){
	    url = window.location.href;
	}
	var result = new RegExp(name + "=([^&]*)", "i").exec(url); 
	return result && unescape(result[1]) || ""; 
    }
    if(inIframe()){
	return;
    }
    var host = 'tracking.keywee.co';
    (function() {	
	var _fbq = window._fbq || (window._fbq = []);
	if (!_fbq.loaded) {
	    var fbds = document.createElement('script');
	    fbds.async = true;
	    fbds.src = '//connect.facebook.net/en_US/fbds.js';
	    var s = document.getElementsByTagName('script')[0];
	    s.parentNode.insertBefore(fbds, s);
	    _fbq.loaded = true;
	}
	_fbq.push(['addPixelId', '297060220477160']);	
    })();
    window._fbq = window._fbq || [];
    window._fbq.push(['track', 'PixelInitialized', {}]);
    var createCookie = function(name, value, days) {
	var expires;
	if (days) {
            var date = new Date();
            date.setTime(date.getTime() + (days * 24 * 60 * 60 * 1000));
            expires = "; expires=" + date.toGMTString();
	}
	else {
            expires = "";
	}
	document.cookie = name + "=" + value + expires + "; path=/; Domain=.hubspot.com";
    }    
    function inIframe () {
	try {
            return window.self !== window.top;
	} catch (e) {
            return true;
	}
    }    
    function getCookie(c_name) {
	if (document.cookie.length > 0) {
            c_start = document.cookie.indexOf(c_name + "=");
            if (c_start != -1) {
		c_start = c_start + c_name.length + 1;
		c_end = document.cookie.indexOf(";", c_start);
		if (c_end == -1) {
                    c_end = document.cookie.length;
		}
		return unescape(document.cookie.substring(c_start, c_end));
            }
	}
	return "";
    }    
    function set_value(key,value){
    	createCookie(key,value,30);
	if(window.localStorage){
	    localStorage.setItem(key,value);
	}
    }
    function get_value(key){
	var value = getCookie(key);
	if(!value){
	    value = localStorage.getItem(key);
	}
	return value;
    }

    ;(function ($, window) {
	
	var intervals = {};
	var removeListener = function(selector) {
	    
	    if (intervals[selector]) {
		
		window.clearInterval(intervals[selector]);
		intervals[selector] = null;
	    }
	};
	var found = 'waitUntilExists.found';
	$.fn.waitUntilExists = function(handler, shouldRunHandlerOnce, isChild) {	    
	    var selector = this.selector;
	    var $this = $(selector);
	    var $elements = $this.not(function() { return $(this).data(found); });
	    
	    if (handler === 'remove') {
		
		// Hijack and remove interval immediately if the code requests
		removeListener(selector);
	    }
	    else {
		
		// Run the handler on all found elements and mark as found
		$elements.each(handler).data(found, true);
		
		if (shouldRunHandlerOnce && $this.length) {
		    
		    // Element was found, implying the handler already ran for all 
		    // matched elements
		    removeListener(selector);
		}
		else if (!isChild) {
		    
		    // If this is a recurring search or if the target has not yet been 
		    // found, create an interval to continue searching for the target
		    intervals[selector] = window.setInterval(function () {
			
			$this.waitUntilExists(handler, shouldRunHandlerOnce, true);
		    }, 500);
		}
	    }
	    
	    return $this;
	};	
    }(jQuery, window));
    var handleOfferEvent = function(kwp_4){
	window._fbq.push(['track', '6027143824480', {'value':'0.00','currency':'USD'}]);		    
	var keywee_conversion_url = '//'+ host +'/pixel.png?kwp_5=25&kwp_6=1&kwp_4='+kwp_4; 
	var image = new Image();
	image.src = keywee_conversion_url;

    }
    var handleConversionEvent = function(kwp_4){
	var email = jQuery.urlParam('email');
	var keywee_conversion_url = '//'+ host +'/pixel.png?kwp_5=25&kwp_6=2&kwp_4='+kwp_4; 
	if(email){
	    keywee_conversion_url += "&kwp_7=" + email
	}
	var image = new Image();
	image.src = keywee_conversion_url;
	window._fbq.push(['track', '6027142360080', {'value':'0.00','currency':'USD'}]);	
    }
    //If we are in first landing page save ad id in cookie
    //If we are in thankyou page send conversion event to keywee and facebook
    //If we are in second landing page send event to keywee
    if(/kwp_4=(\d+)/.test(document.URL)){
	match = /kwp_4=(\d+)/.exec(document.URL);
	if(match[1]){
	    var kwp_4 = match[1];
	    set_value('kwp_4',kwp_4);
	    $(document).ready(function(){
		$(".hs-form").waitUntilExists(function(index,hs_form){
		    $(hs_form).submit(function(){
			handleOfferEvent(kwp_4);
 		    });
		},true)
	    })
	}
    }
    else if(/offers\.hubspot\.com\/thank-you/.test(document.URL)){
	var kwp_4 = get_value('kwp_4');
	if(kwp_4){
	    handleConversionEvent(kwp_4)
	}
    }
    else if(/offers\.hubspot\.com/.test(document.URL) && $("#hs_cos_wrapper_main_form").length){
	var kwp_4 = get_value('kwp_4');
	if(kwp_4){
	    handleOfferEvent(kwp_4);
	}
    }
    if(/hubspot\.com\/podcast/.test(document.URL)){
	var kwp_4 = get_value('kwp_4');
	if(kwp_4){
	    if($(".hs_cos_wrapper").filter(function(index,e) {return $(e).text().indexOf("Thanks") != -1}).length > 0){
		handleConversionEvent(kwp_4);
	    }
	    else{
		handleOfferEvent(kwp_4);
	    }
	}	
    }
})();
