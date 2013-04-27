## Secure SelectorGadget

Loading non-SSL SelectorGadget into SSL websites doesn't work - this is the solution.  It's hosted at [Heroku](http://selectorgadget.herokuapp.com/).

### Usage:

Copy 'n' paste this into a bookmarklet (JS links won't work on Github):

    javascript:(function(){var%20s=document.createElement('div');s.innerHTML='Loading...';s.style.color='black';s.style.padding='20px';s.style.position='fixed';s.style.zIndex='9999';s.style.fontSize='3.0em';s.style.border='2px%20solid%20black';s.style.right='40px';s.style.top='40px';s.setAttribute('class','selector_gadget_loading');s.style.background='white';document.body.appendChild(s);s=document.createElement('script');s.setAttribute('type','text/javascript');s.setAttribute('src','https://selectorgadget.herokuapp.com/js/selectorgadget.js');document.body.appendChild(s);})();
