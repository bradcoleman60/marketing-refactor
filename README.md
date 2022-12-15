# **Marketing Refactor Project**

# **Table of Contents**
1. [Description](#description)
2. [Code Refactor Example](#refactor-example)
4. [Testing](#testing)
5. [Technology Used and Credits](#technology-used-and-credits)
6. [Learnings](#learnings)
7. [About the Author](#about-the-author)
8. [License](#license)

[Visit the Deployed Site](https://bradcoleman60.github.io/marketing-refactor/)


# **Description**

This goal of this project was to: 

1. refactor the HTML and CSS code to make it more accessible and streamlined, and 
2. ensure that use accessibility standards are followed.  

One of the main activities for this project including reviewing the HTML elements.  The original index.html file contained a significant amount of non-semantic elements (for example ```<div>```).  In order to better describe the elements to both the browser and a developer, I replaced such elements with semantic elements.  For example, I replaced ```<div>``` elements with ```<nav>```, ```<section>```, and ```<aside>```.  I used reference materials provided by w3schools.com to aid in this process.  

Additionally, in the original stylesheet.css file I observed several attribute selectors that had identical "properties" and "values".  I was able to consolidate these repetitive selectors into a more generic "class" in order to reduce the code.  

Lastly, the index.htm had several images that did not contain alternative attributes that are useful when complying with accessibility standards.  I reviewed www.blog.hubspot.com to educate myself on web accessibility standards.  These standards contain 4 main principles:

- Perceivable - can visitors understand the content even through the use of screen readers?
- Operable - can visitors use the website without disruption?
- Understandable - can visitors easily understand the sites content? 
- Robust - can visitors easily interpret the website including visitors that use assistive technologies like screen readers?

As a result of my review of these accessibility standards, I included alternative attributes on all image files so that screen readers could interpret them.  

# **Refactor Example**

The following is a representative example of the code that I refactored. In this refactor the navigation links were included in the body element and separate ```<div class="header">``` tag and an unorder list ```<ul>```.   


## Original HTML 
```html
<body>
    <div class="header">
        <h1>Hori<span class="seo">seo</span>n</h1>
        <div>
            <ul>
                <li>
                    <a href="#search-engine-optimization">Search Engine Optimization</a>
                </li>
                <li>
                    <a href="#online-reputation-management">Online Reputation Management</a>
                </li>
                <li>
                    <a href="#social-media-marketing">Social Media Marketing</a>
                </li>
            </ul>
        </div>
    </div>

```


## Refactored HTML

In the refactored html I used the semantic element ```<nav>``` which eliminated the need for defining ```<div class="header">``` and using an unordered lists. 

```html
<header>
    <h1>Hori<span class="seo">seo</span>n</h1>
    <nav>
        <a href="#search-engine-optimization">Search Engine Optimization</a>    
        <a href="#online-reputation-management">Online Reputation Management</a>     
        <a href="#social-media-marketing">Social Media Marketing</a>
    </nav>
</header>
```

# **Testing** 

I wanted to ensure that the alternative attributes for all images discussed above actually worked and could be read by a website reader.  I installed the Chrome Screen Reader add-on and then used the Ctrl-Alt-Z command to test all images.  I am glad I performed this step as it highlighted that I misspelled the word "laptop" in one of the alternative attributes.  Additionally, I noticed that because I used semantic HTML elements, the reader read these more clearly. 

While I was refactoring the code, another process I used to test the code as I progressed, was to "comment out" the original code (in CSS /* */, in HTML <!-- -->) and replace with my suggested improved code.  As such, I was able to test as I progressed through the code. 

# **Technology Used and Credits**

I used many useful references in completing this project including the following.  In particular, I found the layout of the w3schools reference materials to be extremely intuitive and helpful.  They even have a "try me" feature where elements of code can be reviewed and tested. 

- [W3Schools - HTML Code reference:](https://www.w3schools.com/html/default.asp)
- [W3Schools - CSS Code reference:](https://www.w3schools.com/css/default.asp)
- [Hubspot - Web Accessibility Standards:](https://blog.hubspot.com/website/web-accessibility#web-accessibility-standards)
- [Chrome Screen Reader Add-on:](https://chrome.google.com/webstore/detail/screen-reader/kgejglhpjiefppelpmljglcjbhoiplfn/related?hl=en)

# **Learnings**

I had a couple of noteworthy learnings during this project.  First, I confused "refactoring" with reducing or eliminating code.  This caused me to initially eliminate certain specific classes and ID's to streamline the CSS code.  What I didn't realize was that these specific ID's were necessary to ensure that the ```<href>``` worked in the navigation links.  As an aside, I learned that you can not link to a ```<class>```.  

Second, I learned the git workflow.  I performed several add/commit/push commands and this repetition helped me learn the process.  

Lastly, though intuitive and a lesson I have learned throughout my career, collaborating with fellow bootcamp students is very rewarding.  I was able to see different viewpoints and approaches to understanding the concepts of this project.  Additionally, I was exposed to several short cuts and tricks when using VS code.   

# **About the Author**

My name is Brad Coleman. I am fairly new to web development but have considered it a hobby for several years and have hacked my way through learning various aspects including php, html and mysql.  I am currently enrolled in the Cal Berkeley Extension Web Development Boot camp and am excited to learn web development more holistically.  I have spent my earlier career working as a corporate controller / CPA.

- [Linkedin Profile](https://www.linkedin.com/in/brad-coleman-109529/)
- [GitHub Repos](https://github.com/bradcoleman60?tab=repositories)


# **License**

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



