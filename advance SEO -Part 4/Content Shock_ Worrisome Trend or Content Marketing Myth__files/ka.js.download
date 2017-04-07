(function()
{
  var Ka = function()
  {
    this.initialize.apply(this, arguments);
  };
  Ka.prototype =
  {
    url: null,
    initialize: function()
    {
      var script = document.getElementById('ka_tracker');
      if(script)
        this.url = script.src.replace('/ka.js', '/track');
    },
    log: function(data)
    {
      if(this.url == null)
        return;

      var version_id = data[0], post_id = data[1], es_id = data[2];
      var params = [];

      if(post_id && post_id != '')
        params.push('p=' + post_id);

      if(es_id && es_id != '')
        params.push('es=' + es_id);

      if(document.referrer)
        params.push('r=' + encodeURIComponent(document.referrer));

      if(params.length > 0)
      {
        var img = document.createElement('img');
        img.width = img.height = img.style.width = img.style.height = img.style.border = '0';
        img.style.position = "absolute";
        img.style.bottom = "-1px";
        img.src = this.url + '?' + params.join('&');
        document.body.appendChild(img);
      }
    }
  }

  if(typeof _kaq == 'object' && typeof _kaq.length != 'undefined' && typeof _kaq.instance == 'undefined')
  {
    _kaq.instance = new Ka();
    _kaq.push = function(data)
    {
      _kaq.instance.log(data);
      return Array.prototype.push.apply(this, arguments);
    }

    for(var i = 0; i < _kaq.length; i++)
      _kaq.instance.log(_kaq[i]);
  }
})();
