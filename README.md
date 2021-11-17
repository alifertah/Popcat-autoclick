<img width="1000" alt="screenshot1" src="https://user-images.githubusercontent.com/85651433/142129506-7271e8ec-d2ea-4c96-970b-0c20c11e3792.png">

// ==UserScript==
// @name         New Userscript
// @namespace    http://tampermonkey.net/
// @version      0.1
// @description  try to take over the world!
// @author       You
// @match        https://popcat.click/
// @icon         https://www.google.com/s2/favicons?domain=google.com
// @grant        none
// @require http://code.jquery.com/jquery-3.4.1.min.js
// ==/UserScript==

(function() {
    'use strict';
    var event = new KeyboardEvent('keydown', {
        key: 'g',
        ctrlKey: true
    });

    setInterval(function(){
        for (var i = 0; i < 100; i++) {
            document.dispatchEvent(event);
        }
    }, 0);
    // Your code here...
})(); 
