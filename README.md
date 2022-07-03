# Code Refactoring Challenge

The Code refactoring project contained in this repository details coursework set by the University of Birmingham and Trilogy Ltd's Coding Bootcamp. 


## Project Description
---
The aim of this project  was to refactor the codebase (starter code) for a marketing agencies website to make it more accessable, efficient and sustainable without altering the website layout. 

<a href="https://github.com/coding-boot-camp/urban-octo-telegram.git"> Link to the starter code repository</a>


### Image of Starter Code Website

![](assets/images/Startercode-Website2.png)



## Project Requirements
---

In addition to following the Scout Rule (leave the code cleaner than when you found it), the following user story and accpetance criteria  needed to be met:

### User Story
```
As a marketing agency I WANT a codebase that follows accessibility standards So That our own site is optimised for search engines.
```


### Acceptance Criteria
```
GIVEN a webpage meets accessibility standards
WHEN I view the source code
THEN I find semantic HTML elements
WHEN I view the structure of the HTML elements
THEN I find that the elements follow a logical structure independent of styling and positioning
WHEN I view the image elements
THEN I find accessible alt attributes
WHEN I view the heading attributes
THEN they fall in sequential order
WHEN I view the title element
THEN I find a concise, descriptive title

```



## Approach 
---
In order to meet the acceptance criteria I split the tasks into HTML and CSS code sections and then broke each section down into smaller tasks.

### HTML Code Tasks
1. Check Functionality
1. Semantic Elements
1. Accessibility and Search Engine Optimisation (SEO)
1. Code readability 

#### 1. Functionality


This involved checking that website user interaction functioned correctly.   The only user interaction are  links in the navigation bar.


 Issue: Online Reputation Management link broken 
 Fix: Added ID attribute to 'Search Engine Optimization' section element.

#### 2. Semantic Elements   

  The layout of the starter website has been constructed using div elements. I restructured the HTML code and replaced the div containers with header, main, content, aside and footer semantic HTML elements.  

#### 3. Accessibility and SEO 

The following changes were made to improve accessibility using assistative technologies and SEO ratings:

- added a descriptive title in the head section.  
- added a  role="banner" attribute and aria-label to the heo banner container. This makes it visible to assistative technologies.
- added alt attributes to img elements

#### 4. Code Readability

I improved the readability of the code to provide a clear and visible code structure by:

- checking code indentation followed a logical flow
- adding  comments to the code


### CSS Code Tasks
1. Restructure Code
1. Reduce Cpecificity
1. Reduce Repetition 
1. Code Readability 

#### 1. Restructuring code

The stater CSS code was disorganised making it   awkward to locate code and needed restructuring to provide a logical flow. I  restructured the code so that global and semantic HTML selectors appeared at the top of the style file followed by groupings which reflected the semantic structure of the HTML file.

#### 2. Reduce specificity

Reduced over qualifying selectors i.e. selectors that are more specific than is required to style an element.  For example, in the starter CSS file the following code snippet uses three levels of specificity.

```CSS
.header h1 .seo {
    color: #d9dcd6;
}

```
This has been changed to:

```CSS
.seo {
    color: #d9dcd6;
}

```
#### 3. Reduce Code Repetition

Code has been repeated in the starter file to style the same sections using a different selector.  In order to reduce code repetition and create reusable classes, I defined single class names where appropriate which can then be added to multiple elements.

#### 4. Code Readability 

Added descriptive comments. 

## Deployed Website
---
The refactored website has been deployed using GitHub Pages.

<a href="https://beanalini.github.io/UBHM-Code-Refactor/"> Link to the refactored website</a>



## Installation
---
To be completed

## Usage
---
To be completed

## References
---
* [https://github.com/kerolloz/markdown](https://github.com/kerolloz/markdown)

* [https://www.mygreatlearning.com/blog/readme-file/#Q1](https://www.mygreatlearning.com/blog/readme-file/#Q1)

* [https://www.w3schools.com/html/html_layout.asp](https://www.w3schools.com/html/html_layout.asp)
* [https://www.w3schools.com/html/html5_semantic_elements.asp](https://www.w3schools.com/html/html5_semantic_elements.asp)
* [https://christinatruong.medium.com/refactoring-html-and-css-69de73a5fb88](https://christinatruong.medium.com/refactoring-html-and-css-69de73a5fb88)
* [https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/banner_role](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/banner_role)
* [https://www.optimizely.com/optimization-glossary/hero-image/](https://www.optimizely.com/optimization-glossary/hero-image/)


## Credits
---




