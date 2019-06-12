---
---

<script>
    function redirectTo(title, code) {
        
        
          var pathname = ''.replace('[BrowserLangName]', title).replace('[BrowserLangCode]', code);
          if(pathname != '' && window.location['pathname'] != pathname) {
              window.location['pathname'] = pathname;
          }        
        
          var hash = ''.replace('[BrowserLangName]', title).replace('[BrowserLangCode]', code);
          if(hash != '' && window.location['hash'] != hash) {
              window.location['hash'] = hash;
          }        
        
          var href = './[BrowserLangCode]'.replace('[BrowserLangName]', title).replace('[BrowserLangCode]', code);
          if(href != '' && window.location['href'] != href) {
              window.location['href'] = href;
          }        
        
    }
    var userLang = navigator.language || navigator.userLanguage;
    if(false) '';
    
      else if(userLang.indexOf('fr') >= 0) redirectTo('Français', 'fr');
    
      else if(userLang.indexOf('ar') >= 0) redirectTo('Arabe', 'ar');
    
    else redirectTo('Arabe', 'ar');
</script>
