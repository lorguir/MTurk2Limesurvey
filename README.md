# MTurk2Limesurvey

### Description 
As shown by the original repo [ianhussey/MTurk2Limesurvey](https://github.com/ianhussey/MTurk2Limesurvey),

When I went to set up a study using MTurk and Limesurvey I didn't immediately find a solution to pass a workerID from Mechanical Turk to prefill an answer in a Limesurvey question. This is useful to do in order to only pay those who completed the task appropriately. 

A solution for surveys hosted on Qualtrix can be found [here](http://sapir.psych.wisc.edu/wiki/index.php/MTurk). The current code adapts this to work with Limesurvey. NB the question can be set to invisible in Limesurvey so that the participant cannot change the captured workerID.

This code passes html5 validation using https://validator.w3.org, and as such can generate an AMT Layout ID. 

### Usage
`MTurk2Limesurvey.html` should be placed in the AMT requester web interface under `Create > Edit project > Design layout > Source`.

The location of your specific limesurvey installation and the question that is to be prefilled must be specified. Limesurvey answer prefill URLs take the format (more info [here](https://manual.limesurvey.org/Workarounds:_Survey_behaviour#Prefilling_survey_answers_using_the_survey_URL)),

	https://example.com/index.php?r=survey/index&sid=[SURVEY_ID]&newtest=Y&[SGQA]=[PREFILLED_ANSWER_HERE]

For example, (refer to [SURVEY_ID](https://github.com/lorguir/MTurk2Limesurvey/wiki/SURVEY_ID) and [SGQA](https://github.com/lorguir/MTurk2Limesurvey/wiki/SGQA-identifier) on how to locate them)

	https://example.com/index.php?r=survey/index&sid=521424&newtest=Y&521424X3X34=test

If your survey is multi-language, you'll need to specify the language in the link by appending `&lang=[language_code]`
e.g. English survey,

	https://example.com/index.php?r=survey/index&sid=521424&newtest=Y&lang=en&521424X3X34=test

The generated HIT page is extremely simple:

![alt text](https://github.com/ianhussey/MTurk2Limesurvey/blob/master/Screenshot.png "Screenshot")






