## G6 User Testing

# Blog Post:

At this stage in our project, we have developed a medium-fidelity prototype. In order to move forward with the user testing process as well as the development, we focused this prototype on functionality over UI elements. 
Currently, the extension has the following capabilities:
Being able to trigger our extension into any type of YouTube search results page to some capacity (And not triggering for pages that are not youtube search results). This feature will prevent our extension from interfering with other browser use cases. Our extension will not modify the UI or functionality of other browser pages.
Loading UI elements next to individual video search results on the page. On youtube search results pages, our extension will add UI elements to the page. Currently these are two buttons and a test div placed next to the channel name of each video. We ensured that adding our UI elements would not replace any existing UI elements or interfere with any existing functionality. There are currently many bugs associated with this feature that have become apparent through testing.
On our GitHub repo, the code for these features can be found in the following files:
src/manifest.json - This file contains a regex expression to match the URL for any youtube search results page. It works in conjunction with other boilerplate code in the repo
src/content.jsx - This react js file handles the logic for finding the locations in the DOM for any video search results. There is also code that renders App.js next to those video items.
src/App.js - The UI that is rendered next to each video is stored in this file
Other functionalities that we have planned for are currently omitted. An example of one of these features is the ability to read publicly accessible information about a channel source. There is a high chance that these features will not be possible to fully implement in the following week as we have originally designed, but we are looking into alternate implementation methods.
The current UI of the prototype is a wizard-of-oz effect. Since we focused on the background functionality, the UI has a couple mock buttons that do not have any functional purpose. These will be changed to model our design choices and function correctly.    

Examples of Medium Fidelity Prototype:
![Normal 1](/Double-Trouble/images/normal1.PNG)


![Normal 2](/Double-Trouble/images/normal2.PNG)


A normal instance of our prototype.
All videos have a affirm and refute button built into the UI
Even with some extra screen elements and an unrelated search topic, the UI is still modified correctly by the extension.

![Missing](/Double-Trouble/images/missing.PNG)

An example of a bug in our current prototype
One of the videos is missing the extension’s UI elements.

Findings from the user testing sessions
Here are the main takeaways from our testing sessions.
Paging on the search results page: If the user scrolls and loads extra videos (since youtube has an infinite feed on search results), the extension is unable to attach new buttons to the UI. This is one of the highest priority bugs we were able to find from our test users
Firefox and Mac: One of our users found that using firefox and a mac caused the extension to not load for any videos.
Firefox and adblocker (Ublock Origin): This combination also prevents the extension from loading UI for any videos.
Chrome and Mac: Chrome and Mac works for some cases,  but also has some inconsistencies. Our user noticed that there were ads at the top of the screen in this case.
General missing UI elements: Overall, there are some search terms that caused some videos to not load the extension’s UI correctly. We’re unsure as to what the cause is, but it does look like the issue is able to reproduce itself reliably.

Are the findings promising enough that you would like to go ahead with the current functionality of the prototype? (If yes, describe why, if no, describe what changes you are proposing to make.)
    Overall, we will be continuing with the current functional prototype and develop it into our high-fidelity prototype. The UI layout and ordering of buttons didn’t seem to be the main concern of our users in this case. There are a lot of different bugs causing the issue that buttons are not loading at the correct places. It could be a good idea to focus on making the current prototype more consistent at functioning in its ideal environment.
    The next functionalities we plan to implement are more akin to bug fixes. For using google chrome on windows, we plan on loading 100% of the videos’ credibility signal boxes. In addition, we plan on loading videos along with the search results page reloading when the user scrolls to the end of the current feed. Alongside these developments, we will also be focusing on the UI elements of the extension. This part will be important in developing and improving the user-experience of the extension.

