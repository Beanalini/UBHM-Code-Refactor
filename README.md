# Code Refactoring Challenge

The Code refactoring project contained in this repository details coursework set by the University of Birmingham and Trilogy Ltd's Coding Bootcamp. 


## Project Description

The aim of this project  was to refactor the codebase (starter code) for a marketing agencies website to make it more accessible, efficient and sustainable without altering the website layout. 

<a href="https://github.com/coding-boot-camp/urban-octo-telegram.git"> Link to the starter code repository</a>


### Image of Starter Code Website

![](assets/images/Startercode-Website2.png)



## Project Requirements


In addition to following the Scout Rule (leave the code cleaner than when you found it), the following user story and acceptance criteria  needed to be met:

### User Story
```
As a marketing agency I WANT a codebase that follows accessibility
standards So That our own site is optimised for search engines.
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
In order to meet the acceptance criteria I split the tasks into HTML and CSS sections and then broke each section down into smaller tasks.

### HTML Code Tasks

1. Check functionality
1. Check HTML code uses a sematic element structure
1. Check element accessibility and Search Engine (SEO) properties
1. Improve code for readability 

#### 1. Functionality
This involved checking that website user interaction functioned correctly. The only user interaction are links in the navigation bar.

Issue found: Online Reputation Management link broken Fix: Added ID attribute to 'Search Engine Optimization' section element.

#### 2. Semantic Elements
The starter code has used div elements to structure website layout, instead of using semantic HTML elements which convey more meaning to the reader.  I restructured the HTML code and replaced the div containers with header, main, content, aside and footer semantic HTML elements.

#### 3. Element Accessibility and SEO Properties

The following changes were made to improve accessibility using assistative technologies and SEO ratings:

- added a descriptive title in the head section.
- added a role="banner" attribute and aria-label to the heo banner container. This makes it visible to assistative technologies.
- added alt attributes to img elements

#### 4. Code Readability
I improved the readability of the code to provide a clear and visible code structure by:

- checking code indentation followed a logical flow
- adding comments to the code

### CSS Code Tasks
- Restructure code
- Reduce specificity
- Reduce repetition (merge selectors and remove repeated code)
- Improve readability

#### 1. Restructure Code

The stater CSS code was disorganised making it   awkward to locate code and needed restructuring to provide a logical flow. I  restructured the code so that global the body semantic HTML selector appeared at the top of the style file followed by groupings which reflected the semantic structure of the HTML file.

#### 2. Reduce Specificity

I reduced the use of over qualifying selectors i.e. selectors that are more specific than is required to style an element.  For example, in the starter CSS file the following code snippet uses three levels of specificity.

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

The same CSS code has been repeated in the stater code to style HTML elements in the same way using multiple  selectors.  In order to reduce code repetition and create reusable classes, I declared single class selectors containing the required styling properties.  The HTML elements using the same styling now use reusable classes. 

The same font-family property had been set in various selectors in the starter code. To reduce repetition, I placed this property in the body element selector, along with font-size which had been previously been declared using a p element selector.

#### 4. Improve Code Readability 

- Checked code was indented
- Added descriptive comments. 

## Deployed Website

The refactored website has been deployed using GitHub Pages.

<a href="https://beanalini.github.io/UBHM-Code-Refactor/"> Link to the refactored website</a>

## Technologies Used

- HTML
- CSS


## References

* [https://github.com/kerolloz/markdown](https://github.com/kerolloz/markdown)

* [https://www.mygreatlearning.com/blog/readme-file/#Q1](https://www.mygreatlearning.com/blog/readme-file/#Q1)

* [https://www.w3schools.com/html/html_layout.asp](https://www.w3schools.com/html/html_layout.asp)
* [https://www.w3schools.com/html/html5_semantic_elements.asp](https://www.w3schools.com/html/html5_semantic_elements.asp)
* [https://christinatruong.medium.com/refactoring-html-and-css-69de73a5fb88](https://christinatruong.medium.com/refactoring-html-and-css-69de73a5fb88)
* [https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/banner_role](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles/banner_role)
* [https://www.optimizely.com/optimization-glossary/hero-image/](https://www.optimizely.com/optimization-glossary/hero-image/)






