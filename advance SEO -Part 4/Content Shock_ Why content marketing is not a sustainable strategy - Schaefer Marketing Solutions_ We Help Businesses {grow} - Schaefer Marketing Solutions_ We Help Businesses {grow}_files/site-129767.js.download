function anMain() {
	try {

		if (!window.an_category && !window.an_keyword)
			return;
		
		var site = 129767;
		
		var cat = window.an_category || "";
		var kw = window.an_keyword || "";

		var encRegExp = new RegExp("%[0-9A-Fa-f][0-9A-Fa-f]");
		if (!encRegExp.test(cat)) {
			cat = escape(cat);
		}
		if (!encRegExp.test(kw)) {
			kw = escape(kw);	
		}

		var siteref = "";
		if (document.referrer != "" && document.referrer.indexOf(window.location.hostname) == -1) {
		      siteref = ";siteref=" + escape(document.referrer);
		}
		
        document.write("<IFRAME WIDTH='1' HEIGHT='1' MARGINWIDTH='0' MARGINHEIGHT='0' HSPACE='0' VSPACE='0' FRAMEBORDER='0' SCROLLING='no' SRC='http://pbid.pro-market.net/engine?site="+ site +";size=1x1;category="+ cat +";kw="+ kw + siteref +";rnd=(" + new Date().getTime() + " )'></IFRAME>");
	}
	catch (e){
	}
}
anMain();