Montserrat Variable Font
========================

This download contains Montserrat as both variable fonts and static fonts.

Montserrat is a variable font with this axis:
  wght

This means all the styles are contained in these files:
  Montserrat-VariableFont_wght.ttf
  Montserrat-Italic-VariableFont_wght.ttf

If your app fully supports variable fonts, you can now pick intermediate styles
that aren’t available as static fonts. Not all apps support variable fonts, and
in those cases you can use the static font files for Montserrat:
  static/Montserrat-Thin.ttf
  static/Montserrat-ExtraLight.ttf
  static/Montserrat-Light.ttf
  static/Montserrat-Regular.ttf
  static/Montserrat-Medium.ttf
  static/Montserrat-SemiBold.ttf
  static/Montserrat-Bold.ttf
  static/Montserrat-ExtraBold.ttf
  static/Montserrat-Black.ttf
  static/Montserrat-ThinItalic.ttf
  static/Montserrat-ExtraLightItalic.ttf
  static/Montserrat-LightItalic.ttf
  static/Montserrat-Italic.ttf
  static/Montserrat-MediumItalic.ttf
  static/Montserrat-SemiBoldItalic.ttf
  static/Montserrat-BoldItalic.ttf
  static/Montserrat-ExtraBoldItalic.ttf
  static/Montserrat-BlackItalic.ttf

Get started
-----------

1. Install the font files you want to use

2. Use your app's font picker to view the font family and all the
available styles

Learn more about variable fonts
-------------------------------

  https://developers.google.com/web/fundamentals/design-and-ux/typography/variable-fonts
  https://variablefonts.typenetwork.com
  https://medium.com/variable-fonts

In desktop apps

  https://theblog.adobe.com/can-variable-fonts-illustrator-cc
  https://helpx.adobe.com/nz/photoshop/using/fonts.html#variable_fonts

Online

  https://developers.google.com/fonts/docs/getting_started
  https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Fonts/Variable_Fonts_Guide
  https://developer.microsoft.com/en-us/microsoft-edge/testdrive/demos/variable-fonts

Installing fonts

  MacOS: https://support.apple.com/en-us/HT201749
  Linux: https://www.google.com/search?q=how+to+install+a+font+on+gnu%2Blinux
  Windows: https://support.microsoft.com/en-us/help/314960/how-to-install-or-remove-a-font-in-windows

Android Apps

  https://developers.google.com/fonts/docs/android
  https://developer.android.com/guide/topics/ui/look-and-feel/downloadable-fonts

License
-------
Please read the full license text (OFL.txt) to understand the permissions,
restrictions and requirements for usage, redistribution, and modification.

You can use them in your products & projects – print or digital,
commercial or otherwise.

This isn't legal advice, please consider consulting a lawyer and see the full
license for all details.










<html>
  <head>
    <meta charset="utf-8">
    <link rel="stylesheet"
          href="https://fonts.googleapis.com/css?family=Tangerine">
    <style>
      body {
        font-family: 'Tangerine', serif;
        font-size: 48px;
      }
    </style>
  </head>
  <body>
    <div>Making the Web Beautiful!</div>
  </body>
</html>























<script src="https://js-cdn.music.apple.com/musickit/v1/musickit.js"></script>

<head>
 
 <meta name="apple-music-developer-token" content="DEVELOPER-TOKEN">
 <meta name="apple-music-app-name" content="My Cool Web App">
 <meta name="apple-music-app-build" content="1978.4.1">
 
</head>
:

document.addEventListener('musickitloaded', function() {
  // MusicKit global is now defined
  MusicKit.configure({
    developerToken: 'DEVELOPER-TOKEN',
    app: {
      name: 'My Cool Web App',
      build: '1978.4.1'
    }
  });
});

<button id="apple-music-authorize"></button>
<button id="apple-music-unauthorize"></button>


let music = MusicKit.getInstance();

 // This is called with or without authorization: 
 music.player.play();

 // This ensures user authorization before calling play():
 music.authorize().then(function() {
   music.player.play();
 });

 // You can wrap any method to ensure authorization before calling:
 music.authorize().then(function() {
   music.api.library.albums.then(function(cloudAlbums) {
     // user's cloudAlbums
   });
 });