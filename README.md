# M5.2

## Overview

We were tasked to make a given website more accessible and utilizing ARIA as best as we could.

## Sources and Credits

- https://developer.mozilla.org/en-US/docs/Learn/Accessibility/WAI-ARIA_basics
- https://developer.mozilla.org/en-US/docs/Learn/Accessibility/Multimedia

## Accessibility Lab Answers

    Colors:

    The text is difficult to read because of the current color scheme. Can you do a test of the current color contrast (text/background), report the results of the test, and then fix it by changing the assigned colors?

    I changed the background color to a light blue so that the text is more readable. 

    Semantic HTML:

    1. The content is still not very accessible — report on what happens when you try to navigate it using a keyboard.

    Initially it wasn't letting me tab through the options but I fixed that.

    2. Can you update the article text to make it easier for screen reader users to navigate?

    I fixed the header stuff in html by changing the font=5,6,7 stuff to h1,h2,h3 respectively. 
    That fixed all the title stuff.

    3. The navigation menu part of the site (wrapped in <div class="nav"></div>) could be made more accessible by putting it in a proper HTML semantic element. Which one should it be updated to? Make the update.

    I changed it to nav.nav.

    The Images:

    The images are currently inaccessible to screen reader users. Can you fix this?

    I made it accessible to screen reader users by adding alt to the images.
    
    The Audio Player:

    1. The <audio> player isn't accessible to hearing impaired (deaf) people — can you add some kind of accessible alternative for these users?

    I used <details> to make it accessible.

    2. The <audio> player isn't accessible to those using older browsers that don't support HTML audio. How can you allow them to still access the audio?

    I made it so they can download the link themselves if they want and they can play it on whatever device they have.

    The Forms:

    1. The <input> element in the search form at the top could do with a label, but we don't want to add a visible text label that would potentially spoil the design and isn't really needed by sighted users. How can you add a label that is only accessible to screen readers?

    I added this: <form class="search" role="search">
        <input type="search" name="q" placeholder="Search query" aria-label="Search">
        <input type="submit" value="Go!">
      </form>

    2. The two <input> elements in the comment form have visible text labels, but they are not unambiguously associated with their labels — how do you achieve this? Note that you'll need to update some of the CSS rule as well.

    To ensure that the input elements in the comment form are unambiguously associated with their labels, I used the for attribute.

    The Show/Hide Comment Control:

    The show/hide comment control button is not currently keyboard-accessible. Can you make it keyboard-accessible, both in terms of focusing it using the tab key and activating it using the return key?

    Instead of using div class i used button class using aria controls.

    The Table:

    The data table is not currently very accessible — it is hard for screen reader users to associate data rows and columns together, and the table also has no kind of summary to make it clear what it shows. Can you add some features to your HTML to fix this problem?

    I added scope attributes and a caption so users know what they're looking at.






