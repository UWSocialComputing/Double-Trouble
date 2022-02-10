## G3 Low-Fidelity Prototype

# Blog Post:

A - What Is Our Prototype

For our low-fidelity prototype we created a few mock-ups of possible variations of our solution. We used a static image of a YouTube search-results page as a base layer to test multiple small-scale prototypes. Implementing the mock-ups in this manner allowed us to test a variety of different configurations and placements of credibility signals on the UI.
Right now, the ‘wizardry’ comes in the form of the integration of the credibility signals with the YouTube interface. Although our mock-up is not currently an interactive prototype, the elements we have added integrate into the current interface to create an illusion of what the final product might look like. From here, we can integrate feedback to update the appearance and implementation of our solution.

Embedding UI elements into the DOM:
When the prototype is implemented, we will need to modify the DOM in order to insert our credibility signals. The broader project this project is a part of is currently able to insert elements into and modify the YouTube DOM, however the application is not entirely the same. We will have to determine the best methods for integrating our solution with the search-results page.
Gathering data from the Youtube videos:
In order to display information from the videos, we will need to be able to pull data from YouTube. Most of this information should be able to be pulled directly from YouTube, however this is not something that we currently know how to do. We are planning on exploring whether this can be found through the DOM, or if we will need to use some features of the YouTube API.    

B - Prototype Examples
Figure 1: Citations as a Credibility Signal - Grey

![Figure 1: Citations as a Credibility Signal - Grey](/Double-Trouble/images/figg31.JPG)

Figure one shows our first prototype of what credibility signals could look like once inserted into the search results. In this prototype, the design is unobtrusive and meant to integrate seamlessly into the current YouTube UI.

Figure 2: Citations as a Credibility Signals - Colored
![Figure 2: Citations as a Credibility Signals - Colored](/Double-Trouble/images/figg32.JPG)

Figure 2 shows the same credibility signal as the first figure, however in this mock-up we experimented with the addition of color. This makes the signals appear more noticeable and as a stronger signal on the page. We developed this as an opposite to the first example to gain more insight on the design direction of the credibility signals.

Figure 3: Source description as Credibility Signals
![Figure 3: Source description as Credibility Signals](/Double-Trouble/images/figg33.JPG)

Figure 3 shows how additional external information could be shown about the channel who is posting the video. In the examples above, information is pulled from Wikipedia as well as the information section of some of their websites. While this is informative, this may be hard to implement in the timeframe available. We still wanted to get feedback on this possibility in case we are able to implement it.

C- Findings and Results from Wizard of Oz Testing
Our goals going into the test session were to figure out what set of credibility signals and UI decisions would convey the correct information while integrating with the existing Youtube UI. Since the basis and direction of the project is pre-defined, we are mostly using this session to gain more detailed insight of how the extension should behave and look for the best usability and practicality.
    After conducting the testing session, we took away the following ideas:
Information that is easy to find on the video itself shouldn’t appear as credibility signals. Likes (and dislikes before the recent YouTube UI change) and release date are all information that can be easily found on the video page.
This also goes for information that is subjective. The title and video production quality are both aspects that are hard to rigidly quantify. In the test session we determined it was unviable to use these as data for credibility signals.
How to display credibility signals related information (citations, outside sources etc.) is pretty straightforward. It was not the focus of the discussion we had. 
Our credibility signals related to affirming and refuting citations are a great option for helping users determine the credibility of the video. Displaying outside search data is also good information to include. This fills a similar role, and helps give lateral information for users.
An idea to watch for is that crowdsourced citations might be used adversarially. Any user can spam multiple refuting citations if they decide they disagree or dislike a video to skew the video’s citations. While we might not have the time to dive into this, this is a good point to be aware of.
Based on these findings, we are confident in our approach moving forward. The general implementation and content choices will stay mostly the same. The larger changes we will be focusing on moving forward is figuring out a good balance of how unobtrusive/obtrusive the credibility signals should be. Based on feedback from the testing session, we have a few possibilities we will be iterating on and testing out. We may decide to change the format of the credibility signals based on what we think is feasible. An example of this is that some data like the search result ranking are easy to find, and also not always indicative of the credibility of the video. We are very excited for the next steps of this project and how it will develop.
