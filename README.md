# Code Refactor Starter Code

## Description
Per the customer's user story, shown below, our task was to refactor the provided code for the Horiseon landing site to improve its legibility and make it more accesible.

Starter code index.html was improved by implementing semantics HTML elements and alternate text for images to search engine optimization and to enhance user experience for those reading the website through a screen reader. Stylesheet style.css was condensed by merging selectors that serve redundant purposes. Additionally, by evaluating the resulting product through Wave, a Google Chrome extension, https://wave.webaim.org/extension/, for web accessibility evaluation, it determined that the Benefits section's color contrast with the text color was too low. So to enhance contrast, the color for this section was changed to match the rest of the site, resolving the contrast issue and improving the site's aesthetics.

## User story

AS A marketing agency <br />
I WANT a codebase that follows accessibility standards <br />
SO THAT our own site is optimized for search engines

## Acceptance Criteria

GIVEN a webpage meets accessibility standards <br />
WHEN I view the source code <br />
THEN I find semantic HTML elements <br />
WHEN I view the structure of the HTML elements <br />
THEN I find that the elements follow a logical structure independent of styling and positioning <br />
WHEN I view the image elements <br />
THEN I find accessible alt attributes <br />
WHEN I view the heading attributes <br />
THEN they fall in sequential order <br />
WHEN I view the title element <br />
THEN I find a concise, descriptive title <br />

## Screenshot of Deployed Site
![Horiseon Landing Page](./assets/images/HoriseonHeroScreenshot.png)

## Links

GitHub link: https://github.com/nickless192/HoriseonLandingPage

Deployed Page: https://nickless192.github.io/HoriseonLandingPage/

## Code Change Log

### index.html:

- line 7: change title from website to Horiseon
- line 11/26: change div for header
- line 27, 28/50, 51/73, 74/79: change div for section
- line 13/25: change div for nav
- line 29: added id search-engine-optimization
- line 30, 37, 44: add alt text to img
- line 31/37, 38/44, 45/51, 54/60, 61/67, 68/74: change div for article
- line 53, 60, 67: change h3 for h2

### style.css:

- replaced .header h1 for header h1
- replaced .header h1 .seo for header h1 span
- replaced .header div for header nav
- replaced .header div ul for header nav ul
- replaced .header div ul li for header nav ul li
- erged .benefit-lead, .benefit-brand and .benefit-cost into one class, .benefit
- merged .benefit-lead h3, .benefit-brand h3, and .benefit-cost h3 into class .benefit h3
- merged .benefit-lead img, .benefit-brand img and .benefit-cost img into clas .benefit-lead img
- merged classes search-engine-optimization, online-reputation-management, social-media-marketing into class content-info
- merged classes search-engine-optimization img, online-reputation-management img, social-media-marketing img into class content-info img
- merged classes search-engine-optimization h2, online-reputation-management h2, social-media-marketing h2 into class content-info h2
- for class .benefits, changed color #2589bd for #0072bb to enhance legibility (increase contrast)

## Credits

