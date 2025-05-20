# CSE110 Lab 7
The image is in [/admin/tests_passing_36.735.png](/admin/tests_passing_36.735.png).

## Participants
I worked on this solo as I need to just quickly get this done and move on to continuing work on the actual project, 105 midterm prep, the video due tonight, 120 homework due tonight, submitting regrades for another class, et cetera.

## CYU Questions
1. Within a GitHub action that runs whenever code is pushed. This is the only place where the tests are actually automated - the second option runs only on hand run, and the third only tests when development is fully complete, potentially leaving serious bugs in the code.
2. No. This is an internal test and we may pass code into the function, we do not need to simulate user activity to test this.
3. Navigation mode runs a fresh page load from scratch, which measures the page load and post-load state. It doesn't measure anything that runs after the page load, such as user interactions. Snapshot mode gets the current DOM state, which doesn't grab any interactions (it didn't record them), rather fetching a current state view of the site for inspection.
4. Three things:
    a. Add meta tags to describe the document - currently it may have issues such as unreadable text on mobile.
    b. Scale down the image sizes - a 200px wide image does not need to load a 600+px wide base image. It may also help to preload the images since at runtime they take a while to load in.
    c. Change the caching policy to allow for caching larger scripts and JS files, such as the icon and JS files to improve load time.