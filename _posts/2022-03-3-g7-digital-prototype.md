## G7 Digital Prototype

# Blog Post:

### Original Problem:

Our project is aiming to increase factors that viewers can make their decisions based off of by providing new credibility signals in the YouTube search results page. To be more specific, our high-fidelity prototype’s goal is to display credibility signals for each video on a search result page to increase user agency in determining the reputability of a video. 
    Using the results of our user research, we iterated upon designs to come to our final prototype. Due to technical and time limitations, each individual video has its own credibility signal box with the option to expand channel information. The design is meant to be unobtrusive to the user’s search experience, yet allow them to gain more information when wanted.


### Prototype Design:

    Our prototype is currently designed to display the total number of citations as well as the number of citations that have been flagged to refute information in the video. We achieve this through a browser extension that is only active on the youtube search results page. The design of the extension is to add new UI elements to each individual video that appears on the search page. In order to not clutter the original Youtube UI, we designed our UI to take as little space as possible, while still providing ways to view credibility signals.
    The UI that does appear on screen are buttons that allow users to add and view citations that affirm and refute the given video’s information. In order to support this functionality in practice, we are currently limited to modifying existing DOM elements.


### Technical Issues:

    Throughout the process of creating this extension, we’ve run into a couple of technical issues. We found a number of bugs during our medium fidelity testing that raised concerns.
There were many cases where the extension would not appear on screen when expected to. Ads or other extra UI elements modified the overall structure of the page, which would go against our extension’s assumptions about the page layout.

Running our extension on browsers other than Google Chrome and on operating systems other than windows would also cause the extension to behave differently and fail to function in some cases. Adding other extensions like ad blockers caused unexpected behavior as well.
    We also modified the scope and design of the project to suit our time constraints and unfamiliarity with the new technologies we were using. Part of our later development time was dedicated to some of the major bugs in our extension when running on Windows and Google Chrome.


### Demo and Github link:

https://github.com/UWSocialComputing/Double-Trouble-Project

The Readme on this repo has instructions on how to download the extension and test on your browser.


### Screenshots:

![Screenshot of prototype](/Double-Trouble/images/protoscreenshot.PNG)
