# code-refactor-unc

## Description

### Task: 
* Code review and refactor for an existing SEO agency webpage to make it accessible, well-formed, semantically coded, and streamlined.

### User Story 

* **AS A** marketing agency, **I WANT** a codebase that follows accessibility standards **SO THAT** our own site is optimized for search engines.

### Acceptance Criteria

* **GIVEN** improved codebase including HTML, CSS, and assets that:
1. Meets accessibility standards
2. Follows HTML5 standards for semantic HTML
3. Is well-formed / well-structured and commmented for future developer review and improvements
4. Has elements that follow a logical structure independent of styling and positioning
5. Has image elements include alt attributes for accessibility and improved search accessibility
6. Has sequential ordering of heading attributes
7. Contains appropriate (concise, descriptive) meta title
8. Includes general improvements to CSS / HTML while preserving layout and design.

## Optimizations/Change Details:

### Changes in the HTML file, "Agency-Page-Code-Refactor.html"

- [x] 1. Updated _title_ in the _head_ of the page to be meaningful and descriptive.
- [x] 2. Updated _div class="header"_ to semantic element _header_
- [x] 3. Updated _div_ holding the nav _ul_ & _li_'s to semantic element _nav_
- [x] 4. Updated the main content div (_div class="content"_) to semantic element _main_
- [x] 5. Updated sub-divs in the main content div to be sections; removed unnecessary classes and condensed styles appropriately.
- [x] 6. Added missing id for "search-engine-optimization" section nav functionality.
- [x] 7. Updated _div class="benefits"_ to semantic element _aside_
- [x] 8. Updated sub-divs in the aside to be sections; removed unnecessary classes and condensed styles appropriately.
- [x] 9. Updated img tag in the original "benefit-cost" div to remove the unnecessary closing _/img_ tag thereby mirroring the same format as the other images
- [x] 10. Wrapped each image in the _main_ and _aside_ sections in semantic element _figure_
- [x] 11. Updated the _div class="footer"_ to semantic element _footer_
- [x] 12. Changed the _h2_ heading to _h4_ to follow natural declining flow of headings
- [x] 13. Added alt tags to every image on the page except the hero image div 
- [x] 14. Added title attribute to .hero div for improved accessibility to stand-in for aethetic alt text attribute (since image is set as background-image via CSS and thus without alt text attribute setting at this time in CSS3/HTML5) 
**See [Stackoverflow: "CSS background image alt attribute"](https://stackoverflow.com/questions/4216035/css-background-image-alt-attribute)** and answer by [@Randy-Greencorn](https://stackoverflow.com/users/1925485/randy-greencorn)

***Changes in the CSS file, "style.css"

- [x] 14. Changed .header class to apply to semantic element "header" instead
- [x] 15. Updated child h1 as well as span "seo" to parent of "header"
- [x] 16. Updated .header child ul/li's to apply to "header" and semantic element "nav" instead
- [x] 17. Updated .content class to semantic element "main" instead
- [x] 18. Updated .benefits class to semantic element "aside" instead
- [x] 19. Nested sections in aside and styled in single instance, consolidating and removing the need for separate, identically-styled classes of .benefit-lead/.benefit-brand/.benefit-cost
- [x] 20. Styled h3 as a standard page element instead of styling as nested in the "aside", since the "aside" held the only instances of h3
- [x] 21. Styled img in "aside" as single style instance since duplicative styles
- [x] 22. Styled each section in "main" as a single child style instance since duplicative styles, and removed unnecessary classes of .search-engine-optimization/.online-reputation-management/.social-media-marketing
- [x] 23. Styled img in "main" as single style instance since duplicative styles
- [x] 24. Styled h2 as a standard page element instead of styling as nested in the "main", since the "main" held the only instances of h2
- [x] 25. Changed the .footer class to the semantic element "footer" instead 
- [x] 26. Changed the "footer" h2 to be h4 instead to follow natural declination of headings
- [x] 27. Updated order of style elements for global styles first, header second, hero third, and then main section to precede aside section, followed by footer for sake of load-flow, style development best practices, and future specificity as needed/if needed downstream in future updates.
- [x] 28. Added development comments to explain why certain specificity was retained or removed
- [x] 29. Added development comments to indicate semantically organized sections of styles for easier downstream review
- [x] 30. Converted h3 em to px for continuity and downstream comparative edits.

*For change-by-change details, please review [commit log](https://github.com/srmchartroom/code-refactor-unc/commits/master).*
