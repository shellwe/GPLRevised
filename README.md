# GPLRevised Notes

http://themedemos.dottoro.com/features/menu/horizontal-submenu/

Use this for mobile font
https://css-tricks.com/viewport-sized-typography/

Alternatively, you could just add a minimum width to the a tag in mobile so if it goes below a certain size it will wrap around to 1 wide.

Yes another idea for the toggle to work:
http://stackoverflow.com/questions/28101797/jquery-slidetoggle-with-css-media-query

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
