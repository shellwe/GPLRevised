# GPLRevised Notes

http://themedemos.dottoro.com/features/menu/horizontal-submenu/

fade in leaves for menu over .25 seconds with opacity set to 0 (instead of alpha before and set to .8 after so its not so blunt
opacity: 0.25;
transition: all 3s ease;
aldo fade it back when you unhover
https://css-tricks.com/different-transitions-for-hover-on-hover-off/



adding in code to do check for mobile:
http://stackoverflow.com/questions/11381673/detecting-a-mobile-browser
Be sure to wrap it in an isMobile exits if statement so it doesn't get called on every page load
if (null == isMobile)


//Use this to get google analytics

function google_analytics() { ?>
  // Paste your own Google Analytics snippet below
  <script>
    (function(i,s,o,g,r,a,m){i['GoogleAnalyticsObject']=r;i[r]=i[r]||function(){
    (i[r].q=i[r].q||[]).push(arguments)},i[r].l=1*new Date();a=s.createElement(o),
    m=s.getElementsByTagName(o)[0];a.async=1;a.src=g;m.parentNode.insertBefore(a,m)
    })(window,document,'script','//www.google-analytics.com/analytics.js','ga');

    ga('create', 'UA-XXXXXXXX-XX', 'auto');
    ga('send', 'pageview');
  </script>
<?php }
add_action( 'wp_head', 'google_analytics', 10 );
