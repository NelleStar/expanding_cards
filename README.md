building off of a 50 projects 50 days course by Brad Traversy and Florin Pop

Using Vanilla JS, HTML and CSS only to create panels that will expand using event listeners. Flexbox was used to align items neatly on the page.

Could be used for: testimonials, FAQs, photos, trivia/notecards, etc

As a user clicks on the smaller panels the class will switch to "active" thus enlarging it to the full image --- and remove the "active"  class from the previously enlarged panel shrinking it down.

During the course they used inline styling in the HTML file for photos however I was taught to put all styling into the CSS so I switched that around along with making my cards stay in a column rather than laying horizontal. I did this because I wanted the <h3>s to remain showing while removing the <p>s until the user clicked on it. To me, this makes more sense if I wanted to use it for note cards or FAQ so the user can more easily see what they are clicking on rather than guessing. I also took the time to remove pointer events from the h3 or paragraphs to ensure that the panel was the only thing that would register clicks to avoid confusion.

The script.js file is quite simple - We first grab the panels and make a variable using querySelectorAll and forEach panel we listen for a click. Once the user clicks we remove any 'active' class then add the class active to the new panel.