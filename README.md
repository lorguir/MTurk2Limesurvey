# MTurk2Limesurvey

### Description 
_As shown in the original repo [ianhussey/MTurk2Limesurvey](https://github.com/ianhussey/MTurk2Limesurvey),_

When I went to set up a study using MTurk and Limesurvey I didn't immediately find a solution to pass a workerID from Mechanical Turk to prefill an answer in a Limesurvey question. This is useful to do in order to only pay those who completed the task appropriately. 

A solution for surveys hosted on Qualtrix can be found [here](http://sapir.psych.wisc.edu/wiki/index.php/MTurk). The current code adapts this to work with Limesurvey. NB the question can be set to invisible in Limesurvey so that the participant cannot change the captured workerID.

This code passes html5 validation using https://validator.w3.org, and as such can generate an AMT Layout ID. 

### Usage
To capture the completion code in MTurk, refer to [MTurk](https://github.com/lorguir/MTurk2Limesurvey/wiki/MTurk).

To capture the workerID in Limesurvey, refer to [workerID](https://github.com/lorguir/MTurk2Limesurvey/wiki/workerID).

To generate and capture the completion code in Limesurvey, refer to [Completion Code](https://github.com/lorguir/MTurk2Limesurvey/wiki/Completion-Code).
