<!doctype html>
<html dir="ltr" lang="en">
  <head>
    <meta charset="utf-8">
    <style>
      body {
        background: #3F5A8D;
        margin: 0;
      }

      #backgroundImage {
        border: none;
        height: 100%;
        pointer-events: none;
        position: fixed;
        top: 0;
        visibility: hidden;
        width: 100%;

      }

      [show-background-image] #backgroundImage {
        visibility: visible;
      }
    </style>
  </head>
  <body>
    <h1 style="color:red;">hi</h1>
    <iframe id="backgroundImage"
        src="chrome-untrusted://new-tab-page/custom_background_image?url=">
    </iframe>
    <ntp-app></ntp-app>
    <script type="module" src="new_tab_page.js"></script>
    <link rel="stylesheet" href="chrome://resources/css/text_defaults_md.css">
    <link rel="stylesheet" href="shared_vars.css">
  </body>
</html>
