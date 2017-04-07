_satellite.pushAsyncScript(function(event, target, $variables){
  var analytics = _satellite.getVar('ANALYTICS_JS');
  // Skip Intercom otherwise
  analytics.page(_satellite.getVar('PAGENAME'), null, {}, {
    integrations: {
      'Intercom': false
    }
 });
});
