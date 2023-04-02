# A10-Data-Bias

GOAL / HYPOTHESIS

This project is meant to test the throsholds for what is considered "toxic" by the Perspective API. We utilize a given dataset containing examples of online user comments in order to test thresholds.

My theory was that the API may be easily fooled by slight modifications to words or unorthodox sentence structure. This was based on my findings from the original dataset. The reality, as discovered through testing, is far more complicated. The Perspective API seems to interpret changes in grammar and sentence structure very well and will adjust the scoring of sentences fairly accurately based on the changes made. These modification did not change the larger meaning of the comments, keeping identical word choice and direction.

API DOCUMENTATION

The Perspective Comment Analyzer API - From the Google Cloud information page: "The Perspective Comment Analyzer API provides information about the potential impact of a comment on a conversation (e.g. it can provide a score for the "toxicity" of a comment). Users can leverage the "SuggestCommentScore" method to submit corrections to improve Perspective over time. Users can set the "doNotStore" flag to ensure that all submitted comments are automatically deleted after scores are returned." 

Access to this private API was granted by request to the Perspective Developers. If you would like to request access to any of the API tools used in this project, you may make a request at: https://support.perspectiveapi.com/s/?language=en_US
Google Forms Alternative:
https://docs.google.com/forms/d/e/1FAIpQLSdhBBnVVVbXSElby-jhNnEj-Zwpt5toQSCFsJerGfpXW66CuQ/viewform

DATA TYPE LIST



POSSIBLE ISSUES

All testing of the API was done manually, utilizing the VSCode IDE in order to process the given data. By processing data manually, there may be small errors in transfer between applications. This should have a negligable impact on the results of my tests, but the possibility for error is present.
Additionally, all tests were performed without direct access to the API's code or inner workings. However reasonable given the API's proprietary nature, this means a less direct view of the API's actions. As such, any assertions made within this project are simply conclusions drawn from the results of my testing. They should not be taken as factual or descriptive of Perspective API's intended functionality.
