# Testing

This file contains all the different tests performed on the site. It also details the actions taken and any results of those actions.

## [Contents](#contents)

* [Validator Testing](#validator-testing)
* [Manual Testing](#manual-testing)
* [User Testing](#user-testing)
* [Browser Testing](#browser-testing)
* [Device Testing](#device-testing)
* [Lighthouse Report](#lighthouse-report)
* [Fixed Issues](#fixed-issues)
* [Known Issues](#known-issues)

## Validator Testing 

- HTML
  - [index.html](index.html) - No errors were returned when passing through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fpvieira04.github.io%2Fmastermaths%2F).
  - [about.html](about.html) - No errors were returned when passing through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fpvieira04.github.io%2Fmastermaths%2Fabout.html).
  - [contact.html](contact.html) - No errors were returned when passing through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fpvieira04.github.io%2Fmastermaths%2Fcontact.html).
  - [success.html](success.html) - No errors were returned when passing through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fpvieira04.github.io%2Fmastermaths%2Fsuccess.html).
  - [resources.html](resources.html) - No errors were returned when passing through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fpvieira04.github.io%2Fmastermaths%2Fresources.html).
  - [404.html](404.html) - No errors were returned when passing through the official [W3C validator](https://validator.w3.org/nu/?doc=https%3A%2F%2Fpvieira04.github.io%2Fmastermaths%2F404.html).

- CSS
  - No errors were found when passing through the official [(Jigsaw) validator](https://jigsaw.w3.org/css-validator/validator?uri=https%3A%2F%2Fpvieira04.github.io%2Fmastermaths%2F&profile=css3svg&usermedium=all&warning=1&vextwarning=&lang=en#css).

## Manual Testing

- Header
  - "Skip to content" link works perfectly on every page.
  - Easily targetable using the keyboard, as intended.
  - Unable to target any other way, also as intended.

- Navigation Bar
  - All links work as expected.
  - Navigation bar is responsive.
  - Always appears at the top of the page.

- Landing Page
  - Fully responsive.
  - In desktop mode, the first section is responsive until the media queries trigger tablet mode.
  - In tablet mode, the right hand side reliably stays at the top, while the photo and tutor info is placed beneath.
  - Call to action button is responsive and works as expected.
  - Bottom two sections have responsive text and call to action buttons work as expected.

- About Page
  - Fully responsive.
  - The layout in desktop and mobile mode is the same.
  - The call to action at the bottom of the page works as intended.

- Contact Page
  - Fully responsive.
  - Has a maximum width and then responsively adjusts width until the madeia query for tablets triggers.
  - In tablet mode, the first part of the form is displayed on top and the textbox is displayed beneath.
  - The submit button works as intended. The user is only directed to the success page until all required fields have been adequately filled out.

- Success Page
  - Fully responsive.
  - The layout in desktop and mobile mode is the same.
  - Call-to-action buttons work as intended.

- Resources Page
  - Fully responsive.
  - Layout changes between desktop and mobile modes for the GCSE and A Level sections.
  - In Desktop mode, the images are on the left hand side while the description of the site is on the right.
  - In mobile mode, this changes so that the image appears above its description.

- 404 Page
  - Fully responsive.
  - Displayed error message always fits on the page.
  - Call-to-action button works as expected.

- Footer
  - Fully responsive.
  - Anchor tag works as expected.
  - Social Media links work as expected.
  - Layout stays the same between desktop and mobile mode.
  - On smaller screens, space between elements is reduced with no change to icon dimensions or text size.

- Keyboard-only Users
  - All navigation, buttons, anchors and input fields can be fully scrolled through by pressing the tab key or shift+tab.
  - All elements the user is able to focus can be interacted with by pressing neter.
  - Fully functional and working as intended.

- Screen-reader Users
  - Test carried out using NVDA. 
  - All links when tabbed through have accurate descriptions.

## User Testing

I asked a real user to open my website on dektop. They used a mouse to navigate and this person has no accessibility requirements. This is how it went.

- User opens the MasterMaths website and reads the tagline.
- User then reads the tutor information section and scrolls down.
- User reads the heading for sections two and three of the Landing Page and then scrolls back up.
- They click on the about link in the navigation bar and read the quote.
- They laugh and nod their head.
- User scrolls down and reads about half of the about-process section.
- User scrolls down further to the about-travel section and comments on the map of serviceable areas - "Oh is that where you can travel to?"
- User clicks on the "Check Availability" call-to-action button.
- User sees the contact form and then navigates to resources via the navigation bar.
- They click on the image expecting it to open the website(they commented on it) and it opens in a new tab.
- The user closes the new tab and closes the MasterMaths tab.

## Browser Testing
Manual Testing was further done on other browsers. These browsers were chosen becasue, as found by [statcounter](https://gs.statcounter.com/browser-market-share), they are the most popular browsers in the world.

### Desktop Browsers
- Chrome
  - Developed using this browser. No issues detected.
- Edge
  - No issues detected.
- Safari
  - Issue detected on Landing Page - .tutor-pic takes up more than 50% of the screen width and squashes .tutor-info. Significantly different to Chrome, Edge and Firefox. (FIXED)
  - Extra unwanted styling added to select fields in contact form. (FIXED)
  - Footer always appears at the bottom of the viewport. Should only appear at the bottom of the page. (FIXED)
  - a tags should have rounded borders. On safari they do not.
- Firefox
  - Submit input on contact form says "Submit Query" instead of just "Submit". (FIXED)
  - Some spacing is missing in the contact page and on the resources page. (FIXED)
  - Shows outline on png used as background image for select field. (FIXED)
- Opera
  - No issues detected.

### Tablet and Mobile Browsers

The tests for the following browsers can be found in the [device testing](#device-testing) section.

The following are the most popular browsers for tablet and mobile:

- Android (Tablet and Mobile) - Browser now out of circulation and has not been added to any recent android devices. Unable to find a device to test.
- Chrome (Android)
- Safari (iOS Mobile)
- Safari (iOS Tablet)
- Samsung Internet (Amdroid Mobile)

## Device Testing

While the device toolbar in Chrome Developer Tools was used throughout the development process, further manual tests were carried out on various physical devices visiting the [live website](https://pvieira04.github.io/mastermaths).

Android Devices

- One Plus 6 - Chrome
  - No issues, behaves as intended.
- Google Pixel 7 - Chrome
  - No issues, behaves as intended.
- Galaxy A33 5G - Samsung Internet
  - No issues, behaves as intended.
- Galaxy Tab A8 - Samsung Internet
  - Layout of contact.html in portrait mode has the two main sections of the form side by side.
  - I ideally would want them to be orientated just like in mobile mode; small issue.

iOS Devices (all using Safari Browser for iOS)

- iPhone 13 mini
  - No issues detected
- iPhone 14 Pro
  - No issues detected
- iPad (10th gen)
  - Same issues as on Safari on Mac
  - In tablet mode, .tutor-pic takes up more than 50% of the screen width
  - Extra styling added to select fields
  - All these issues now fixed.

## Lighthouse Report

### Initial Report

![Initial Lighthouse Report](./assets/media/lighthouse/lighthouse-report-initial.png)

### Actions

All actions were derived from addressing the opportunites outlined in the lighthouse report.

1. Added aria-label to external links in footer (Accessibility).
2. Converted image in index.html to webp format (Performance).
3. Added meta descriptions to all html pages (SEO).
4. Replaced Fontawesome CDN with manual installation of Fontawesome and deleted uneccessary styling rules (Performance).
5. Converted images in resouces.html to webp format and changed resolution appropriately (Performance).
   * Between the before and after shown below, the performance score stayed the same but the Cumulative Layout Shift changed by 0.004.
   * [Resources Mobile Before](./assets/media/lighthouse/lighthouse-report-resources-mobile-before.png)
   * [Resources Mobile After](./assets/media/lighthouse/lighthouse-report-resources-mobile-after.png)

### Results

![Final Lighthouse Report - Landing Page Desktop](./assets/media/lighthouse/lighthouse-report-after.png)

Under the Diagnostics section in the Lighthouse report, a warning was given to do with caching. The warning was called "Serve static assets with an efficient cache policy". After doing my research, it seems that since I am using Github Pages to deploy this project, I am unable to change the cache time which is [always set to 600 seconds](https://webapps.stackexchange.com/questions/119286/caching-assets-in-website-served-from-github-pages#comment143669_119294). Thus, this is one issue I am unable to address unless I change my deployment process.

Across all HTML pages, mobile rendering of the Lighthouse tool results in an equal or lower score for performance when compared to mobile.

Resulting Investigation:
- Cumulative Layout Shift(CLS) is either the same or higher on mobile when compared to desktop. This could affect the Performance score.
- The problem with this hypothesis is that the about page has an the same CLS value on mobile and desktop renders of the tool (0.042).
- Across desktop renders of all pages, the First Contentful Paint and Largest Contentful Paint are at 0.5 seconds, whereas mobile renders of all pages have a First Contentful Paint of 1.7 and a Largest Contentful Paint of 1.7 or higher.
- Unable to find a reason why mobile renders are slower across the board.

## Fixed Issues

## Known Issues

Firefox browser has some layout changes compared to all other browsers that I tested. I do not know how to fix this.