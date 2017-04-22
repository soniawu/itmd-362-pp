# Production Problem 10: A/B Testing on the Cheap

## The Problem

Locate an interface component on a website that you use frequently that you think could be improved. The improvement should be minor.

Take a screenshot of the interface on both a mobile and desktop device. Then, sketch or illustrate your alternate/"b" test. Finally, describe modification and the HTML, CSS, and JavaScript that you would need to write in order to conduct the test.

## Deliverables

* Screenshots of the interface component on mobile and desktop, placed in this directory (`pp-10/`)
The following screen shots are attached:

1. UHC_mobile.png     - the mobile page
2. UHC_desktop_1.png  - the desktop page when screen is in large size
3. UHC_desktop_2.png  - the desktop page when screen is in about 600px

* Sketch or illustrate (e.g., in Photoshop) your alternate/"b" test, placed in this directory (`pp-10/`)

UHC_mobile_B.png  -  sketch for mobile

The desktop change will be in text description.

* A text description of the modification, and a description of the HTML, CSS, and JavaScript that you would need to write for the test (you do *not* have to write the actual HTML, CSS, and JavaScript, however)

This is the United Healthcare member login site. The mobile version overall looks good. The subtitle blue color bar, stating "mobile" is not necessary. I would remove the bar and relocate the "myuhc" up next to the logo with smaller font size, keep the Spanish button the same place. Also make the login box bigger.

For this part I would change 
HTML - move the <button> tag from the subtitle bar to the main box, move the <h> for myuhc to the header, remove the subtitle bar.

CSS - remove rules apply to the subtitle bar, increase login box size.

JS - may or may not have codes to handle subtitle bar. check, if any, remove them. the event listener for Spanish should be independent, no impact.

The desktop version is not responsive. The whole picture will show only when the window size is big enough, about 700px (see UHC_desktop_1). When window size decrease, need horizontal scroll bar(see UHC_desktop_2). For the simple page like this, we can avoid the scroll bar in a big range of screen size by defining the box width as percentage instead of fix size.

Change for this can be made only in CSS for the box width, plus may be a few adjusted layout.