(function(){var k=this;function ba(a){a=a.split(".");for(var b=k,c;c=a.shift();)if(null!=b[c])b=b[c];else return null;return b}
function l(a){var b=typeof a;if("object"==b)if(a){if(a instanceof Array)return"array";if(a instanceof Object)return b;var c=Object.prototype.toString.call(a);if("[object Window]"==c)return"object";if("[object Array]"==c||"number"==typeof a.length&&"undefined"!=typeof a.splice&&"undefined"!=typeof a.propertyIsEnumerable&&!a.propertyIsEnumerable("splice"))return"array";if("[object Function]"==c||"undefined"!=typeof a.call&&"undefined"!=typeof a.propertyIsEnumerable&&!a.propertyIsEnumerable("call"))return"function"}else return"null";
else if("function"==b&&"undefined"==typeof a.call)return"object";return b}
function n(a){return"string"==typeof a}
;/*
 gapi.loader.OBJECT_CREATE_TEST_OVERRIDE &&*/
var p=window,q=document,ca=p.location;function da(){}
var ea=/\[native code\]/;function r(a,b,c){return a[b]=a[b]||c}
function fa(a){for(var b=0;b<this.length;b++)if(this[b]===a)return b;return-1}
function ga(a){a=a.sort();for(var b=[],c=void 0,d=0;d<a.length;d++){var e=a[d];e!=c&&b.push(e);c=e}return b}
function u(){var a;if((a=Object.create)&&ea.test(a))a=a(null);else{a={};for(var b in a)a[b]=void 0}return a}
var x=r(p,"gapi",{});function y(a,b){this.width=a;this.height=b}
y.prototype.ceil=function(){this.width=Math.ceil(this.width);this.height=Math.ceil(this.height);return this};
y.prototype.floor=function(){this.width=Math.floor(this.width);this.height=Math.floor(this.height);return this};
y.prototype.round=function(){this.width=Math.round(this.width);this.height=Math.round(this.height);return this};var ha="constructor hasOwnProperty isPrototypeOf propertyIsEnumerable toLocaleString toString valueOf".split(" ");function ia(a,b){for(var c,d,e=1;e<arguments.length;e++){d=arguments[e];for(c in d)a[c]=d[c];for(var f=0;f<ha.length;f++)c=ha[f],Object.prototype.hasOwnProperty.call(d,c)&&(a[c]=d[c])}}
;function ja(a,b){var c=ka;Object.prototype.hasOwnProperty.call(c,a)||(c[a]=b(a))}
;var la=String.prototype.trim?function(a){return a.trim()}:function(a){return a.replace(/^[\s\xa0]+|[\s\xa0]+$/g,"")};
function z(a,b){return a<b?-1:a>b?1:0}
;var A;a:{var ma=k.navigator;if(ma){var na=ma.userAgent;if(na){A=na;break a}}A=""};var E=window.yt&&window.yt.config_||window.ytcfg&&window.ytcfg.data_||{},F=["yt","config_"],G=k;F[0]in G||!G.execScript||G.execScript("var "+F[0]);for(var H;F.length&&(H=F.shift());)F.length||void 0===E?G[H]&&G[H]!==Object.prototype[H]?G=G[H]:G=G[H]={}:G[H]=E;var I;I=r(p,"___jsl",u());r(I,"I",0);r(I,"hel",10);function oa(){var a=ca.href,b;if(I.dpo)b=I.h;else{b=I.h;var c=RegExp("([#].*&|[#])jsh=([^&#]*)","g"),d=RegExp("([?#].*&|[?#])jsh=([^&#]*)","g");if(a=a&&(c.exec(a)||d.exec(a)))try{b=decodeURIComponent(a[2])}catch(e){}}return b}
function pa(a){var b=r(I,"PQ",[]);I.PQ=[];var c=b.length;if(0===c)a();else for(var d=0,e=function(){++d===c&&a()},f=0;f<c;f++)b[f](e)}
function J(a){return r(r(I,"H",u()),a,u())}
;var qa=Array.prototype.indexOf?function(a,b,c){return Array.prototype.indexOf.call(a,b,c)}:function(a,b,c){c=null==c?0:0>c?Math.max(0,a.length+c):c;
if(n(a))return n(b)&&1==b.length?a.indexOf(b,c):-1;for(;c<a.length;c++)if(c in a&&a[c]===b)return c;return-1},ra=Array.prototype.filter?function(a,b,c){return Array.prototype.filter.call(a,b,c)}:function(a,b,c){for(var d=a.length,e=[],f=0,g=n(a)?a.split(""):a,h=0;h<d;h++)if(h in g){var m=g[h];
b.call(c,m,h,a)&&(e[f++]=m)}return e};
function sa(a,b){for(var c=1;c<arguments.length;c++){var d=arguments[c],e=l(d);if("array"==e||"object"==e&&"number"==typeof d.length){var e=a.length||0,f=d.length||0;a.length=e+f;for(var g=0;g<f;g++)a[e+g]=d[g]}else a.push(d)}}
;var K=r(I,"perf",u());r(K,"g",u());var ta=r(K,"i",u());r(K,"r",[]);u();u();function M(a,b,c){b&&0<b.length&&(b=ua(b),c&&0<c.length&&(b+="___"+ua(c)),28<b.length&&(b=b.substr(0,28)+(b.length-28)),c=b,b=r(ta,"_p",u()),r(b,c,u())[a]=(new Date).getTime(),b=K.r,"function"===typeof b?b(a,"_p",c):b.push([a,"_p",c]))}
function ua(a){return a.join("__").replace(/\./g,"_").replace(/\-/g,"_").replace(/\,/g,"_")}
;function va(a){if(a.classList)return a.classList;a=a.className;return n(a)&&a.match(/\S+/g)||[]}
function wa(a,b){var c;a.classList?c=a.classList.contains(b):(c=va(a),c=0<=qa(c,b));return c}
function xa(a,b){a.classList?a.classList.add(b):wa(a,b)||(a.className+=0<a.className.length?" "+b:b)}
function ya(a,b){a.classList?a.classList.remove(b):wa(a,b)&&(a.className=ra(va(a),function(a){return a!=b}).join(" "))}
;var za=u(),N=[];function O(a){throw Error("Bad hint"+(a?": "+a:""));}
N.push(["jsl",function(a){for(var b in a)if(Object.prototype.hasOwnProperty.call(a,b)){var c=a[b];"object"==typeof c?I[b]=r(I,b,[]).concat(c):r(I,b,c)}if(b=a.u)a=r(I,"us",[]),a.push(b),(b=/^https:(.*)$/.exec(b))&&a.push("http:"+b[1])}]);
var Aa=/^(\/[a-zA-Z0-9_\-]+)+$/,Ba=[/\/amp\//,/\/amp$/,/^\/amp$/],Ca=/^[a-zA-Z0-9\-_\.,!]+$/,Da=/^gapi\.loaded_[0-9]+$/,Ea=/^[a-zA-Z0-9,._-]+$/;function Fa(a,b,c,d){var e=a.split(";"),f=e.shift(),g=za[f],h=null;g?h=g(e,b,c,d):O("no hint processor for: "+f);h||O("failed to generate load url");b=h;c=b.match(Ga);(d=b.match(Ha))&&1===d.length&&Ia.test(b)&&c&&1===c.length||O("failed sanity: "+a);return h}
function Ja(a,b,c,d){function e(a){return encodeURIComponent(a).replace(/%2C/g,",")}
a=Ka(a);Da.test(c)||O("invalid_callback");b=La(b);d=d&&d.length?La(d):null;return[encodeURIComponent(a.g).replace(/%2C/g,",").replace(/%2F/g,"/"),"/k=",e(a.version),"/m=",e(b),d?"/exm="+e(d):"","/rt=j/sv=1/d=1/ed=1",a.a?"/am="+e(a.a):"",a.c?"/rs="+e(a.c):"",a.f?"/t="+e(a.f):"","/cb=",e(c)].join("")}
function Ka(a){"/"!==a.charAt(0)&&O("relative path");for(var b=a.substring(1).split("/"),c=[];b.length;){a=b.shift();if(!a.length||0==a.indexOf("."))O("empty/relative directory");else if(0<a.indexOf("=")){b.unshift(a);break}c.push(a)}a={};for(var d=0,e=b.length;d<e;++d){var f=b[d].split("="),g=decodeURIComponent(f[0]),h=decodeURIComponent(f[1]);2==f.length&&g&&h&&(a[g]=a[g]||h)}b="/"+c.join("/");Aa.test(b)||O("invalid_prefix");c=0;for(d=Ba.length;c<d;++c)Ba[c].test(b)&&O("invalid_prefix");c=P(a,"k",
!0);d=P(a,"am");e=P(a,"rs");a=P(a,"t");return{g:b,version:c,a:d,c:e,f:a}}
function La(a){for(var b=[],c=0,d=a.length;c<d;++c){var e=a[c].replace(/\./g,"_").replace(/-/g,"_");Ea.test(e)&&b.push(e)}return b.join(",")}
function P(a,b,c){a=a[b];!a&&c&&O("missing: "+b);if(a){if(Ca.test(a))return a;O("invalid: "+b)}return null}
var Ia=/^https?:\/\/[a-z0-9_.-]+\.google\.com(:\d+)?\/[a-zA-Z0-9_.,!=\-\/]+$/,Ha=/\/cb=/g,Ga=/\/\//g;function Ma(){var a=oa();if(!a)throw Error("Bad hint");return a}
za.m=function(a,b,c,d){(a=a[0])||O("missing_hint");return"https://apis.google.com"+Ja(a,b,c,d)};
var Q=decodeURI("%73cript"),Na=/^[-+_0-9\/A-Za-z]+={0,2}$/;function Oa(a,b){for(var c=[],d=0;d<a.length;++d){var e=a[d];e&&0>fa.call(b,e)&&c.push(e)}return c}
function Pa(){var a=I.nonce;if(void 0!==a)return a&&a===String(a)&&a.match(Na)?a:I.nonce=null;var b=r(I,"us",[]);if(!b||!b.length)return I.nonce=null;for(var c=q.getElementsByTagName(Q),d=0,e=c.length;d<e;++d){var f=c[d];if(f.src&&(a=String(f.nonce||f.getAttribute("nonce")||"")||null)){for(var g=0,h=b.length;g<h&&b[g]!==f.src;++g);if(g!==h&&a&&a===String(a)&&a.match(Na))return I.nonce=a}}return null}
function Qa(a){if("loading"!=q.readyState)Ra(a);else{var b=Pa(),c="";null!==b&&(c=' nonce="'+b+'"');q.write("<"+Q+' src="'+encodeURI(a)+'"'+c+"></"+Q+">")}}
function Ra(a){var b=q.createElement(Q);b.setAttribute("src",a);a=Pa();null!==a&&b.setAttribute("nonce",a);b.async="true";(a=q.getElementsByTagName(Q)[0])?a.parentNode.insertBefore(b,a):(q.head||q.body||q.documentElement).appendChild(b)}
function Sa(a,b){var c=b&&b._c;if(c)for(var d=0;d<N.length;d++){var e=N[d][0],f=N[d][1];f&&Object.prototype.hasOwnProperty.call(c,e)&&f(c[e],a,b)}}
function Ta(a,b,c){Ua(function(){var c;c=b===oa()?r(x,"_",u()):u();c=r(J(b),"_",c);a(c)},c)}
function R(a,b){var c=b||{};"function"==typeof b&&(c={},c.callback=b);Sa(a,c);var d=a?a.split(":"):[],e=c.h||Ma(),f=r(I,"ah",u());if(f["::"]&&d.length){for(var g=[],h=null;h=d.shift();){var m=h.split("."),m=f[h]||f[m[1]&&"ns:"+m[0]||""]||e,B=g.length&&g[g.length-1]||null,C=B;B&&B.hint==m||(C={hint:m,b:[]},g.push(C));C.b.push(h)}var L=g.length;if(1<L){var D=c.callback;D&&(c.callback=function(){0==--L&&D()})}for(;d=g.shift();)Va(d.b,c,d.hint)}else Va(d||[],c,e)}
function Va(a,b,c){function d(a,b){if(L)return 0;p.clearTimeout(C);D.push.apply(D,t);var d=((x||{}).config||{}).update;d?d(f):f&&r(I,"cu",[]).push(f);if(b){M("me0",a,S);try{Ta(b,c,B)}finally{M("me1",a,S)}}return 1}
a=ga(a)||[];var e=b.callback,f=b.config,g=b.timeout,h=b.ontimeout,m=b.onerror,B=void 0;"function"==typeof m&&(B=m);var C=null,L=!1;if(g&&!h||!g&&h)throw"Timeout requires both the timeout parameter and ontimeout parameter to be set";var m=r(J(c),"r",[]).sort(),D=r(J(c),"L",[]).sort(),S=[].concat(m);0<g&&(C=p.setTimeout(function(){L=!0;h()},g));
var t=Oa(a,D);if(t.length){var t=Oa(a,m),v=r(I,"CP",[]),w=v.length;v[w]=function(a){function b(){var a=v[w+1];a&&a()}
function c(b){v[w]=null;d(t,a)&&pa(function(){e&&e();b()})}
if(!a)return 0;M("ml1",t,S);0<w&&v[w-1]?v[w]=function(){c(b)}:c(b)};
if(t.length){var aa="loaded_"+I.I++;x[aa]=function(a){v[w](a);x[aa]=null};
a=Fa(c,t,"gapi."+aa,m);m.push.apply(m,t);M("ml0",t,S);b.sync||p.___gapisync?Qa(a):Ra(a)}else v[w](da)}else d(t)&&e&&e()}
function Ua(a,b){if(I.hee&&0<I.hel)try{return a()}catch(c){b&&b(c),I.hel--,R("debug_error",function(){try{window.___jsl.hefn(c)}catch(d){throw c;}})}else try{return a()}catch(c){throw b&&b(c),c;
}}
x.load=function(a,b){return Ua(function(){return R(a,b)})};var Wa=-1!=A.indexOf("Opera"),T=-1!=A.indexOf("Trident")||-1!=A.indexOf("MSIE"),Xa=-1!=A.indexOf("Edge"),Ya=-1!=A.indexOf("Gecko")&&!(-1!=A.toLowerCase().indexOf("webkit")&&-1==A.indexOf("Edge"))&&!(-1!=A.indexOf("Trident")||-1!=A.indexOf("MSIE"))&&-1==A.indexOf("Edge"),Za=-1!=A.toLowerCase().indexOf("webkit")&&-1==A.indexOf("Edge");function $a(){var a=k.document;return a?a.documentMode:void 0}
var ab;a:{var bb="",cb=function(){var a=A;if(Ya)return/rv\:([^\);]+)(\)|;)/.exec(a);if(Xa)return/Edge\/([\d\.]+)/.exec(a);if(T)return/\b(?:MSIE|rv)[: ]([^\);]+)(\)|;)/.exec(a);if(Za)return/WebKit\/(\S+)/.exec(a);if(Wa)return/(?:Version)[ \/]?(\S+)/.exec(a)}();
cb&&(bb=cb?cb[1]:"");if(T){var db=$a();if(null!=db&&db>parseFloat(bb)){ab=String(db);break a}}ab=bb}var eb=ab,ka={};
function fb(a){ja(a,function(){for(var b=0,c=la(String(eb)).split("."),d=la(String(a)).split("."),e=Math.max(c.length,d.length),f=0;0==b&&f<e;f++){var g=c[f]||"",h=d[f]||"";do{g=/(\d*)(\D*)(.*)/.exec(g)||["","","",""];h=/(\d*)(\D*)(.*)/.exec(h)||["","","",""];if(0==g[0].length&&0==h[0].length)break;b=z(0==g[1].length?0:parseInt(g[1],10),0==h[1].length?0:parseInt(h[1],10))||z(0==g[2].length,0==h[2].length)||z(g[2],h[2]);g=g[3];h=h[3]}while(0==b)}return 0<=b})}
var gb;var hb=k.document;gb=hb&&T?$a()||("CSS1Compat"==hb.compatMode?parseInt(eb,10):5):void 0;var ib;if(!(ib=!Ya&&!T)){var jb;if(jb=T)jb=9<=Number(gb);ib=jb}ib||Ya&&fb("1.9.1");T&&fb("9");function kb(){return ba("gapi.iframes.getContext")()}
function lb(){return ba("gapi.iframes.SAME_ORIGIN_IFRAMES_FILTER")}
;function mb(){var a=document;return n("yt-subscribe-card")?a.getElementById("yt-subscribe-card"):"yt-subscribe-card"}
;function nb(a){var b=a.offsetWidth,c=a.offsetHeight,d=Za&&!b&&!c;if((void 0===b||d)&&a.getBoundingClientRect){var e;a:{try{e=a.getBoundingClientRect()}catch(f){e={left:0,top:0,right:0,bottom:0};break a}T&&a.ownerDocument.body&&(a=a.ownerDocument,e.left-=a.documentElement.clientLeft+a.body.clientLeft,e.top-=a.documentElement.clientTop+a.body.clientTop)}return new y(e.right-e.left,e.bottom-e.top)}return new y(b,c)}
;function ob(a){try{var b=pb,c=lb();a.register("msg-hovercard-subscription",b,c)}catch(d){}}
function pb(a){if(a){a=!!a.isSubscribed;var b=mb();a?ya(b,"subscribe"):xa(b,"subscribe");a?xa(b,"subscribed"):ya(b,"subscribed")}}
;var U;
function qb(){var a;a=mb();var b;b:{b=9==a.nodeType?a:a.ownerDocument||a.document;if(b.defaultView&&b.defaultView.getComputedStyle&&(b=b.defaultView.getComputedStyle(a,null))){b=b.display||b.getPropertyValue("display")||"";break b}b=""}if("none"!=(b||(a.currentStyle?a.currentStyle.display:null)||a.style&&a.style.display))a=nb(a);else{b=a.style;var c=b.display,d=b.visibility,e=b.position;b.visibility="hidden";b.position="absolute";b.display="inline";a=nb(a);b.display=c;b.position=e;b.visibility=d}a=
{width:a.width,height:a.height};kb().ready(a,null,void 0);a=lb();kb().addOnOpenerHandler(ob,null,a)}
U="function"==l(qb)?{callback:qb}:qb||{};
if(U.gapiHintOverride||"GAPI_HINT_OVERRIDE"in E&&E.GAPI_HINT_OVERRIDE){var rb;var V=document.location.href;if(-1!=V.indexOf("?")){var V=(V||"").split("#")[0],sb=V.split("?",2),W=1<sb.length?sb[1]:sb[0];"?"==W.charAt(0)&&(W=W.substr(1));for(var tb=W.split("&"),X={},ub=0,vb=tb.length;ub<vb;ub++){var Y=tb[ub].split("=");if(1==Y.length&&Y[0]||2==Y.length){var Z=decodeURIComponent((Y[0]||"").replace(/\+/g," ")),wb=decodeURIComponent((Y[1]||"").replace(/\+/g," "));Z in X?"array"==l(X[Z])?sa(X[Z],wb):X[Z]=
[X[Z],wb]:X[Z]=wb}}rb=X}else rb={};var xb=rb.gapi_jsh;xb&&ia(U,{_c:{jsl:{h:xb}}})}R("gapi.iframes:gapi.iframes.style.common",U);}).call(this);
