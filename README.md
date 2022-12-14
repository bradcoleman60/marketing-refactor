# marketing-refactor

## Summary

This goal of this project was to 

1) refactor the HTML and CSS code to make it more accessible and streamlined, and 
2) ensure that use accessibilty standards are followed.  

One of the main activities for this project including reviewing the HTML elements.  The original index.html file contained a significant amount of non-semnatic elements (for example <div>).  In order to better discribe the elements to both the browser and a developer, I replaced such elements with semantic elements.  For example, I replaced <div> elements with <nav>, <section>, and <aside>.  I used reference materials provided by w3schools.com to aid in this process.  

Additionally, in the original stylesheet.css file I observed several attribute selectiors that had identical "properties" and "values".  I was able to consolidate these repetitive selectors into a more generic "class" in order to reduce the code.  

Lastly, the index.htm had several images that did not contain alternative attributes that are useful when compling with accessibilty standards.  I reviewed www.blog.hubspot.com to educate myself on web accessibitiy standards.  These standards contain 4 main principles:

1) Perceivable - can visitors undertand the content even through the use of screan readers?
2) Operable - can visitors use the website without disruption?
3) Understandable - can vistors easily understand the sites content? 
4) Robust - can vistors esaily interpret the website including vistors that use assistive technologies like screen readers?

As as result of my review of these accessibility standards, I included alternative attributes on all image files so that screen readers could interpret.  

## Testing 

I wanted to ensure that the alternative attributes for all images dicussed above actually worked and could be read by a website reader.  I installed the Chrome Screen Reader add-on and then used the Ctrl-Alt-Z command to test all images.  I am glad I performed this step as it higlighted that I misspelled the word "laptop" in one of the alternative attributes.  Additionally, I noticed that because I used semantic HTML elements, the reader read these more clearly. 

While I was refactoring the code, another prcoess I used to test the code as I progressed, was to "comment out" the original code (in CSS /* */, in HTML <!-- -->) and replace with my suggested improved code.  


## Installation

N/A

## Usage

This website provides notes and information on three coding langauges on creating a website - HTML, CSS and Javascript.  It also contains console.log information - Please open yoiur browser's "Inspect" console (Console Dev Tools) to view the console.log information. 


## Credits

HTML Code:                      https://www.w3schools.com/html/default.asp
CSS Code:                       https://www.w3schools.com/css/default.asp
Web Accessibilty Standards:     https://blog.hubspot.com/website/web-accessibility#web-accessibility-standards
Chrome Screen Reader Add-on:    https://chrome.google.com/webstore/detail/screen-reader/kgejglhpjiefppelpmljglcjbhoiplfn/related?hl=en



## License

MIT License

Copyright (c) 2022 Brad Coleman

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.



