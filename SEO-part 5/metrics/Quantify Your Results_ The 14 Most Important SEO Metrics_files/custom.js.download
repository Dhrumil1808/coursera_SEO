jQuery(function($) {

	// general:
	
	if( /Android|webOS|iPhone|iPad|iPod|BlackBerry/i.test(navigator.userAgent) ) {
	
		var isMobile = true;
		
	} else {
	
		var isMobile = false;
	
	};
	
	
	// homepage:
	
	if ( $( 'body' ).hasClass( 'page-template-page_box-php' ) ) {
	
		$('.qs-box-form-search .compare').toggle(function(){
		
			$('.qs-box-form-search').addClass('qs-box-form-searchs');
			$('.qs-box-form-search .additional').show();
			$(this).find('.symbol').html('-');
			$(this).find('.text').html('Close');
		
		}, function() {
		
			$('.qs-box-form-search').removeClass('qs-box-form-searchs');
			$('.qs-box-form-search .additional').hide();
			$(this).find('.symbol').html('+');
			$(this).find('.text').html('Compare Up to 3 Competitors');
		
		});
		
		$('.qs-box-form-search .compare').before('<p class="error"></p>');
		$('#search-url').focus();
		
		// input required fallback:
		
		function hasHtml5Validation () {
		
			return typeof document.createElement('input').checkValidity === 'function';
		
		};

		if (hasHtml5Validation()) {
		
			$('.qs-box-form-search form').submit(function(e) {
			
				if (!this.checkValidity()) {
				
					e.preventDefault();
					
					$('#search-url').focus();
					$('.qs-box-form-search .error').text('Please enter in a URL');
					$('.qs-box-form-search .error').css('display','block');
				
				};
			
			});
		
		}
	
	};
	
	
	// tabs:
	
	if( $('#popular-tabs').length ) {
	

		$('#popular-tabs div').hide();
		$('#popular-tabs div:first').show();
		
		$('#popular-tabs #pt-nav a').click(function(){
			$('#popular-tabs #pt-nav a').removeClass('active');
			$('#popular-tabs div').hide();
			
			$(this).addClass('active');
			currentTab = $(this).attr('href');
			$(currentTab).show();
			
			return false;
		});
	
	};
	
	
	// wap:
	
	if( $('#comments').length ) {
	
		var wap = $('#wap');
		var wap_closed = $.cookie('_quicksprout_wap_closed');
		
		if(!isMobile && !wap_closed) { 
			
			function checkScrollingWap(event) {
			
				$('#comments:in-viewport').each(function() {
				
					if ($(wap).hasClass('hidden')) {

						$(wap).removeClass('hidden');
						
					};
				
				});
				
			}
			
			$(window).bind('scroll', checkScrollingWap);
			
			$('#wap .close').click(function(){
			
				$(wap).addClass('closed');
				$.cookie('_quicksprout_wap_closed', '1', { expires: 90, path: '/' });
			
			});
			
		} else {
		
			$(wap).css('display','none');
		
		}
		
	};
	
	
	// twitter:
	
	if( $('.tweet-js-me').length ) {
	
		function loadTwitter() {
		
			if (typeof (twttr) != 'undefined'){
			
				twttr.widgets.load();
			
			} else {
			
				$.getScript('http://platform.twitter.com/widgets.js');
			
			}
		
		};
	
		function checkScrollingTwitter(event) {
		
			$('.tweet-js-me:in-viewport').each(function() {
			
				$(this).find('a').addClass('twitter-share-button');
				$(this).removeClass('tweet-js-me');
				
				loadTwitter();
			
			});
			
		}
		
		$(window).bind('load', checkScrollingTwitter);
		$(window).bind('scroll', checkScrollingTwitter);
		
	};
	
	
	$('.bt-mobile-list').click(function(){
		$(this).toggleClass('active');
		$('#list-mobile').toggle();
	});
	
	
	// label to placeholder:
	
	$('.qs-label-to-placeholder').each(function() {
	
		var label = $(this).find('label');
		var input = $(label).next('input');
		
		$(input).attr('placeholder',label.text());
		$(label).hide();
		
		if (navigator.appVersion.indexOf("MSIE 9.")!=-1) {
		
			$(input).attr('value',label.text());
			
			$(input).focus(function(){
			
				if($(this).val() == $(this).attr('placeholder')){
				
					$(this).val('');
				
				}
			
			});
			
			$(input).blur(function(){
			
				if($(this).val() == '') {
				
					$(this).val($(this).attr('placeholder'));
				
				}
			
			});
		
		};
	
	});
	
	
	// others:
	
	var top = 0;
	
	$("#content div.post").last().css({border:"none"});
	
	$(window).load(function(){
	
		if( $('.scroll-element').length ) {
			
			top = $('.scroll-element').offset().top;
			//top = $('.scroll-element').offset().top - parseFloat($('.scroll-element').css('marginTop').replace(/auto/, 0));
		}
		
	});

	
	$(window).scroll(function (event) {
		
		if( top ) {
			var y = $(this).scrollTop();
			
			if (y >= top) {
			  $('.scroll-element').addClass('fixed');
			  //$('.scroll-element').text( "scrollTop: " + y + " | top: " + top );
			} else {
			  $('.scroll-element').removeClass('fixed');
			  //$('.scroll-element').text( "scrollTop: " + y + " | top: " + top );
			}
		}
	
	});
  
  
	$(".ts-video-testimonial").click(function() {
			$.fancybox({
				'padding'		: 0,
				'autoScale'		: false,
				'transitionIn'	: 'none',
				'transitionOut'	: 'none',
				'title'			: this.title,
				'width'		    : 680,
				'height'		: 400,
				'href'			: this.href.replace(new RegExp("watch\\?v=", "i"), 'v/'),
				'type'			: 'swf',
				'swf'			: {
				'wmode'		        : 'transparent',
				'allowfullscreen'	: 'true'
			}
		});
		
		return false;
	});
	
	
	
	if( $('#cntfrm').length ) {
	
		$('#cntfrm').validate();
	
			$('#ErrorMsg').hide() ;
	
			$('.ReserveYourConfidentialBtn').click(function(e) {
	
				e.preventDefault() ;
	
				
	
				if($('#Name').val() == 'Name')
	
					$('#Name').val('');
	
				//if($('#Phone').val() == 'Phone')
	
				//	$('#Phone').val('');
	
				if($('#Email').val() == 'Email Address')
	
					$('#Email').val('');
	
				if($('#Link').val() == 'Website URL')
	
					$('#Link').val('');
	
				if($('#Name').val() == 'Name')
	
					$('#Name').val('');
	
				
	
				
	
				$('#cntfrm').trigger('submit');
	
				//$('#myfrm').trigger('submit');
	
				return false ;
	
		}) ;	// $('.SubmitForm').click
	
		
	
		$('#cntfrm').submit(function() {
	
				if( !$('#Name').hasClass('error') && !$('#Email').hasClass('error') && !$('#Link').hasClass('error') ) //&& !$('#Revenue').hasClass('error')
	
				{
	
					showForm(false) ;
	
					//this.form.reset() ;
	
					//setTimeout('showForm(true)', 5000) ;
	
				}
	
				else
	
					return false ;
	
			}) ;	// $('#frmInspect').submit
	
	
	
		showForm(true) ;
	
	}
  
});

var $jq = jQuery.noConflict();

function showForm(ShowForm) {

		if (ShowForm)

		{

		

			$jq('#EmailForm').show() ;

			$jq('#ThanksMsg').hide() ;

			document.cntfrm.reset() ;

		}

		else

		{

			$jq('#EmailForm').hide() ;

			$jq('#ThanksMsg').show() ;

		}

	}	// function showForm(ShowForm)

	

	function PhoneFormat(obj)

	{

		var re= /\D/;

		// test for this format: (xxx)xxx-xxxx

		var re2 = /^\({1}\d{3}\)\d{3}-\d{4}/; 

		// test for this format: xxx-xxx-xxxx

		//var re2 = /^\d{3}-\d{3}-\d{4}/;

		

		for (i=0; i<obj.value.length;i++){

		var num=obj.value;

		

		var newNum;

		 if (num != "" && re2.test(num)!=true){

		   if (num != ""){

			 while (re.test(num)){

			 num = num.replace(re,"");

			 }

		   }

		

		  if (num.length != 10){

			alert('Please enter a 10 digit phone number');

			//obj.select();

			break;

			}

		   else {

			 // for format (xxx)xxx-xxxx

			// newNum = '(' + num.substring(0,3) + ')' + num.substring(3,6) + '-' + num.substring(6,10);

			 // for format xxx-xxx-xxxx

			  newNum = num.substring(0,3) + '-' + num.substring(3,6) + '-' + num.substring(6,10);

			 obj.value=newNum;

			 }

		   }

		  }

	}

function validateForm()
{
	var x=document.forms["cntfrm"]["Email"].value;
	var atpos=x.indexOf("@");
	var dotpos=x.lastIndexOf(".");
	if (atpos<1 || dotpos<atpos+2 || dotpos+2>=x.length)
	  {
	  alert("Not a valid e-mail address");
	  return false;
	  }
}

function process_login(a) {
	if(window.location.host == 'qs.truewinterstudios.com') {
		var finalUrl = 'http://qs.truewinterstudios.com/';
	} else {
		var finalUrl = 'http://www.quicksprout.com/';
	}

    a.preventDefault();
    var b = $jq("#log").val(),
        c = $jq("#pwd").val();
    $jq.post(finalUrl+"wp-content/themes/quicksprout/login.php", {
        username: b,
        user_pass: c,
        user_login: "1"
    }, function (a) {
        "failed" == a.response ? login_failed(a.reason) : login_success(b, c)
    }, "json")
}

function login_success(a, b) {
    $jq(".stor-username").val($jq("#log").val());
    $jq(".stor-user_pass").val($jq("#pwd").val());
    $jq(".login-redirect").submit()
}

function login_failed(a) {
	var finalUrl = 'http://www.quicksprout.com/';
    $jq(".fancybox-wrap").animate({
        left: "53%",
		marginLeft: "-150px"
    }, 50, function () {
        $jq(".fancybox-wrap").animate({
            left: "47%"
        }, 50, function () {
            $jq(".fancybox-wrap").animate({
                left: "51%"
            }, 50, function () {
                $jq(".fancybox-wrap").animate({
                    left: "49%"
                }, 50, function () {
                    $jq(".fancybox-wrap").animate({
                        left: "50%",
                        marginLeft: "-150px"
                    }, 50)
                })
            })
        })
    });
    "" === a && (a = "Fields are empty.");
    a = a.replace("<strong>ERROR</strong>:", "");
    a = a.replace("The password you entered for the username", "Wrong Password.");
    a = a.replace("is incorrect.", "");
    a = a.replace("Lost your password", "Forgot Password");
    a = a.replace(finalUrl+"wp-login.php?action=lostpassword", finalUrl+"lost-password/\" class=\"open-box fancybox.ajax\" data-width=\"300\" data-height=\"240");
    $jq(".replaceit").html('<span class="o errorLogin">' + a + "</span>")
}

/*var validator = new FormValidator('cntfrm', [{
    name: 'Name',
    display: 'required',    
    rules: 'required'
},
{
    name: 'req',
    display: 'required',    
    rules: 'required'
}, {
    name: 'alphanumeric',
    rules: 'alpha_numeric'
}, {
    name: 'password',
    rules: 'required'
}, {
    name: 'password_confirm',
    display: 'password confirmation',
    rules: 'required|matches[password]'
}, {
    name: 'Email',
    rules: 'valid_email'
},
{
    name: 'Link',
    display: 'required',    
    rules: 'required'
},
 {
    name: 'minlength',
    display: 'min length',
    rules: 'min_length[8]'
}], function(errors, event) {
    if (errors.length > 0) {
        // Show the errors
    }
});*/
