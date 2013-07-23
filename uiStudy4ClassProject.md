# Web UI Framework Study for Class Project

The note presents a short research on selecting UI platform for TalkAbout app. There are many factors affects an UI platform selection and this is a selection for implementing very specific app-TalkAbout. 

## Assumption:
  
- The user of this app is mainly nordic, who discovers some discussion opportunities near by, and he decides to join them or he creates one on the spot. It is spontaneous. The user is less like to plan everything out in front of desk. This is a mobile app.
- The app is location driven, which means the device has GPS function. Many desktop and notebook can not provide the location information.
- It is for this cleass project. It will developed by the people in this class project, not for an enterprise which can be more academic, and implemented by a outsourcing group. The skillset and available time for developing this project is fixed.
- The software stack can be changed after the class.

## References:
[Cage Match!](http://css.dzone.com/articles/sencha-touch-v-jquery-mobile)
[from Quora](http://www.quora.com/Mobile-Web-Development/Which-is-a-better-platform-to-use-JQuery-Mobile-or-Twitter-Bootstrap)
[BootStrap-3](http://designmodo.com/twitter-bootstrap-3/) 
[BootStrap-3 changes](https://github.com/twitter/bootstrap/pull/6342)

## List of platforms under consideration 
- Bootstrap: it is popular for web based app and is part of class leason which need to learn.
- jQuery Mobile (jqm): built on top of jQuery and JS
- Sencha: has strong support for touch and gesture.
- Native app (iPhone and Android) or other tools: [Titanium and Alloy](http://www.appcelerator.com)

## Review 
Disclaimer: I only have limited hands on experience of Bootstrap and JQM, and some experience on Android.
     
### JQM 
- required a many jQuery libraries and then the Mobile platform on top of it. 
- It uses HTML for layout.
- It has pre-defined themes.
- It has better web commpatible than Sencha.

### Bootstrap

- Supports [LESS](http://lesscss.org/) which simplifies the CSS development. 
- Responsive feature is part of basic package, it makes layout easy. There are many layout service to speedup the BS-2 layout. It is very productive for web apps.
- BS-2 use jQuery, it can work with JQM but there are some issues.

- Bootstrap-3 will be released in about 3 weeks, which claims "mobile first". It has few additional enhancements.
- There is additinal layout service from Bootply.com, which provides very smooth layout experience. 
- The grid systems are fluid by default.

### Sencha

- better graphic (SVG) support.
- use javascript for layout.
- It has strong MVC pattern.
- It has native wrappers for iOS and Android.
- Swipe and gestures work.

### Native

- better native look and feel.
- easier to integrate with location api, it is likely to have better performance. 


