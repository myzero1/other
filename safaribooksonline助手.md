
Tampermonkey脚本

```js
  // ==UserScript==
  // @name         New Userscript
  // @namespace    http://tampermonkey.net/
  // @version      0.1
  // @description  try to take over the world!
  // @author       You
  // @match        http://www.cnblogs.com/*
  // @match        https://www.safaribooksonline.com/*
  // @grant        none
  // @require    http://libs.baidu.com/jquery/1.9.0/jquery.min.js
  // ==/UserScript==

  //clear style
  $("#sbo-rt-content").css("max-width","100%");
  $(".annotator-wrapper").css("font-size","600%");
  $(".annotator-wrapper").css("font-weight","bold");
  //$("#sbo-rt-content .annotator-wrapper pre").css("cssText", "white-space:normal!important;");
  //$("#sbo-rt-content .annotator-wrapper pre").css("cssText", "white-space:pre-wrap!important;");
  $("#sbo-rt-content .annotator-wrapper pre").css("cssText", "word-wrap:break-word!important;white-space:pre-wrap!important;");

  //clear docment  
  $(".sbo-site-nav").remove();
  $(".pagefoot").remove();
  $(".sbo-menu-top").remove();
  $(".toc-menu").remove();
  $(".sbo-nav-top").remove();
  $(".interface-controls-top").remove();
  $(".sbo-nav-bottom").remove();
  $("#js-subscribe-nag").remove();

```



加上chrome插件，打印（打印当前网页），https://chrome.google.com/webstore/detail/idfnpgjblkahngbondojabhffkkdekbd?utm_source=chrome-app-launcher-info-dialog
