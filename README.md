# Lab 3: Bootstrap Study Buddy

You are turning a plain HTML page into a styled, responsive website using Bootstrap 4. The starter file has all the content already written and none of the styling. Your job is to add the Bootstrap classes and the custom CSS that make it look like a real product page.

Follow the Lab 3 handout on Canvas. It walks through every section with the lab videos. This README covers setup, submission, and grading.

## What is in this repo

- `index.html` is the unstyled starter page. All sections are already there and commented: Nav Bar, Title, Features, Testimonials, Pricing, Call To Action, Footer.
- `css/styles.css` is empty except for one comment. All of your custom CSS goes here.
- `images/` holds the photos and logos you will need. Do not rename these files.

Bootstrap 4.5.2 is already linked from a CDN in the `<head>`, and jQuery, Popper, and Bootstrap JS are linked at the bottom of `<body>`. Leave those alone.

## Before you start

1. Clone this repo to your computer and open the folder in VS Code.
2. Rename `index.html` to `LastnameLab3.html` using your actual last name. Do this first. If you skip it you will hit problems later when you put the site on your account website.
3. Open the file with Live Server so you can see your changes as you save.

## What you need to do

The handout has the full walkthrough. The short version:

1. Copy the navbar from Lecture 14 into the section commented `<!-- Nav Bar -->`.
2. Link your stylesheet with `<link rel="stylesheet" href="css/styles.css">` placed below the Bootstrap CSS link. Order matters. Bootstrap loads first, your styles override it.
3. Use the Bootstrap grid to split the title section so the text and buttons take the left half and the phone image takes the right half on large screens.
4. Add two Google Fonts and apply them to your headings and nav.
5. Add Font Awesome icons to the download buttons, the features section, and the footer.
6. Build the testimonials section as a Bootstrap carousel with working previous and next controls.
7. Build the pricing section as three cards in a card deck that stack correctly on tablet and phone.
8. Use z-index and positioning to tuck the phone image behind the features section.
9. Add a media query at the bottom of your CSS so the page still works on a phone.
10. Style the call to action and footer.

Make the site your own. Pick your own colors, fonts, and icons rather than copying the ones in the handout screenshots. Part of your grade is customization.

## Font Awesome

Font Awesome requires a free account. Register with your email, then paste the kit script they send you into the `<head>` of your HTML. The kit code is tied to your account, so use your own rather than a classmate's.

## Submitting

Commit and push your work to this repo before the deadline. The last push before the deadline is what gets graded.

From the VS Code terminal:

- `git add .`
- `git commit -m "Lab 3 complete"`
- `git push`

Check the repo on github.com afterward to confirm your HTML, your CSS, and the images folder are all there. If your page renders locally but not from the repo, something did not get pushed.

## Grading (54 points)

| Criteria | Points |
|---|---|
| Working website that renders correctly | 25 |
| Customized colors | 4.83 |
| Customized fonts | 4.83 |
| Customized icons | 4.83 |
| Customized testimonials | 4.83 |
| Customized images | 4.83 |
| No obvious minor issues | 4.85 |

A site that renders but has major formatting problems, usually from a broken CSS link or Bootstrap not loading, earns half credit on the first row. Nothing submitted, or a page that will not render, earns zero there.

"No obvious minor issues" means no dead links, no missing images, images at a reasonable size, and a page that looks finished.

## If something breaks

- Nothing you wrote in CSS is showing up. Check that your `<link>` to `css/styles.css` is in the `<head>` and that the path matches your folder structure.
- The hamburger menu does not open. The three `<script>` elements at the bottom of the page are missing or commented out. Bootstrap needs that JavaScript.
- Images are broken. Check spelling and capitalization in the `src` path. GitHub is case sensitive even if your laptop is not.
- The carousel arrows do nothing. The `href` on the controls has to match the `id` you gave the carousel div.
