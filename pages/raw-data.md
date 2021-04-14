---
title: "Experimental Data"
---
## Raw Data from the Think Aloud Protocols in 2021

In 2021, we conducted an experiment with 6 developers using the [Think Aloud Protocol](https://psycnet.apa.org/record/1980-24435-001). The collected raw data are available under the following sections. For more details check our publications. Note, that all textual material provided here is in Hungarian, except from several parts which are provided in English as examples.

### Transcription of the Videos

We obtained video material of total length of 33 hours and 57 minutes.
Each video frame was composed of two parts: the participants screen area and video footage.
We created a transcription of each recorded video in form of subtitles (SRT format) with additional information about gestures and other activities of the participants such as relevant changes of facial expression, gesticulation, and other environment factors (this is similar to subtitles for the deaf and hard of hearing for movies).
After this step, all the videos could be edited to remove identifying information, that is video and voice of the participant, and leave only the screen capture part with the transcript.

The transcripts can be downloaded from [here](https://github.com/InteractiveFaultLocalization/think-aloud-utils/tree/iFL2021/video-logs).
We also translated several samples of these subtitles to English, which can be downloaded [here](https://github.com/InteractiveFaultLocalization/think-aloud-utils/tree/iFL2021/video-logs/translated%20samples).

You could inspect these samples in human-readable format in the following blocks.

{% include collapse.html title="Transcript of debugging session without additional tools (2021-02-22_09-46-27-ENG, sample)"
content="
The participant starts the exercise. He says <em>'well I'm gonna run the base...'</em> he looks down at the instructions <em>'or... next to the green run button from the arrow pointing down we choose the taskA configuration from the dropdown menu.'</em><br/>
He double checks the task, sighs, and repeats it while finding the appropriate menu. <em>'From the dropdown menu choose... okay.'</em><br/>
He clicks on the TaskA test and runs it.<br/>
He makes observations while waiting. <em>'Now I'm waiting for it to finish running. I can see this is a maven project, though I could guess that from the src main java and from pom.'</em><br/>
<em>'It's interesting though, because the jre system library says Java 1.6, but here it was run with 1.7'</em> he adds, then clears his throat.<br/>
<em>'Well anyway, I'll look into this'</em> he says before looking up to see the finished test.<br/>
Looking at the Console log he continues. <em>'Okay here I can see... it deleted them.'</em><br/>
He pauses for a moment to adjusts his glasses.<br/>
<em>'I'll search for... in math the... erm NumberUtils.java'</em> he says while clicking the folders in the Project Explorer.<br/>
He opens the file he was looking for and continues. 'But otherwise you should search for it in the test, but for this java class (unintelligible)... you can make sense of the test.'<br/>
He starts opening other files from the Explorer while adding 'I will open these and I'll search for the taskCreatNumber task.'<br/>
He seems to have difficulty finding the task, however, and mumbles 'This is a constructor... testToInt... string...' then decides to change tactics.<br/>
'This is a relatively long file so I will search with CTRL+F.'<br/>
He opens the Find/Replace window.<br/>
'Umm... I hope this will work.'<br/>
'I'm looking for the testCreat' he explains while typing it into the window, 'but anyway in Eclipse there should be an option to see the functions...' He starts looking for the settings.<br/>
'In Window, maybe Editor... Show view, and here is one called... not Project, buuut... Expressions maybe?' He clicks it. It's not the one he wanted.<br/>
'Nope nope nope nope' he realizes, and clicks away to continue looking elsewhere. <br/>
'I want to see somewhere the... what this contains' he goes on, but decides to give up for fear of losing too much time.<br/>
'Never mind, I'll just search for it instead of wasting more time on it, because I don't know how they planned this one and a half hour.'"
%}

{% include collapse.html title="Transcript of debugging session with additional tools (2021-02-24_13-40-45-ENG, sample)"
content="
'Oookay, now let's see... what's going on here'<br/>
The participant starts the task by clicking on the test case.<br/>
While it loads he thinks aloud about his next steps. 'Well I don't know; I don't think coverage can help us much right now.' He scratches his head. 'I'm not trying to write a new test. Well okay, clearly we can look at what it shows...' he stops as he only sees an empty table under Coverage, 'oh, yeah especially if... If this is not how you do it at all...' he muses, 'but by default did it not...?'<br/>
He comes to a realization.<br/>
'It didn't run, well never mind then.  Well then what to do, what does it say...' He sighs deeply while looking down at the task description.<br/>
'Yes, coverage as, [click] on coverage all, on coverage all.' He figures out what to.<br/>
'Good, click JUnit test, mhm' he muses while clicking in the menu.<br/>
He then looks down at the task description again.<br/>
'Call graph... it's super interesting though that, that Atlas plugin. It's possible it won't be able to help in this exact situation, I'll look into it in a second...'"
%}

{% include collapse.html title="Transcript of debugging session with additional tools (2021-02-26_09-23-24-ENG, sample)"
content="
The participant starts the task.<br/>
'Okay, well erm, now we'll try to use this iFL - oh I still haven't selected the project. Okay, here are the failed tests... iFL' he mumbles while clicking through various windows and popups.<br/>
'Erm, yes, so now I selected the project in iFL, erm, okay.'<br/>
He waits for the program to load before continuing. 'We're gonna test what this tool is good for, now that I know how... how it works. Well this puts it in a different context now that I know how it works.' <br/>
He starts making faces because the loading still hasn't finished.<br/>
'But sadly the... the tool is not too... tool fast' He proceeds to laugh at his own pun.<br/>
'Whoops' he exclaims once the results finally show up on the screen.<br/>
'Now it's showing us something' he notes, looking through the results. 'Maybe if it's in the project root it will load automatically?' he wonders. 'Because, erm... Because yesterday, well never mind, I'll click on Load scores again.' And he does.<br/>
'Uuuuuh,' he keeps clicking around in the tool. 'Okay, well it says that... based on the score' he explains as he tries to put the scores in order. 'I'll put it in order from top to bottom. There's only one problem with this, which is that the Signature is ... mhm.' He notices that the Signature field is too long to fit into the cell, and thus is not visible in its entirety. It can be scrolled through to the end with a mouse though. 'Well it's... scrollable' he concludes.<br/>
'The error will be at Fraction' he deduces looking at the results window. He wants to see additional information. <br/>
'The Fraction's test ... yeah... let's look at this... erm. I double click it, right? Then it will jump to it? Does it also open it? Or just...if it's open will it jump to it?' he tries it. 'No, it also opens it, awesome!'<br/>
'Uuuh, okay, so theoretically this...' he keeps looking at the plugin '... in this test there are errors... fraction, fraction, fraction...' he mumbles trying to figure out what to do next.<br/>
He looks through the code. 'Let's see... Name: reduce. It's a bit lower, okay, it's quite big.' He starts clicking through the Fault Localization results. 'Well... Well this is... maybe there won't be errors in (unintelligible)' he mumbles. 'But these are, pretty big...pretty big methods.'<br/>
'GetNumerator, there won't be errors in this one' he explains as he clicks on it. 'I will go on and lower its score... How did it go? Maybe you just need to...' It takes a little time to figure out how to modify the score. He right clicks. 'That's it... erm... Context feedback... good' <br/>
He opens the Context based feedback window.<br/>
'So I will lower this, I won't modify the others yet, but I'll lower this, <em>'cause this definitely won't have errors.'<br/>
'Getter' he says and continues clicking.<br/>
He finds an issue he's not happy with. <br/>
'Mutable ... oh yes, here with the ordering - I would report a bug with iFL that if you modify the context, then the ordering will disappear.' Then he keeps searching. 'Denominator... erm... I could do multiple ones at the same time' he muses about checking the result items. 'Erm Fraction, here well, I suppose there won't be any errors here either' he says and moves on. 'Erm... getReduceFraction... here the rows are a little skewed, Position, but whatever, I found these, this is fine.'"
%}

{% include collapse.html title="Transcript of debugging session with additional tools (, sample)"
content="
"
%}


### Handouts

At the beginning of each debugging session we gave [printed handouts](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/handouts/tasks.pdf) to the participants which contained the following information:

+ ID of the task (A, B, etc.)
+ Failing test case(s)
+ Short description (one sentence) of the failure
+ Execution instruction about the test suite

Before warm-up and debugging session of the feature phase we provided further information about the main features of the three IDE plug-ins, which were introduced during this phase.
At the beginning of the debugging sessions in the feature phase and use-case phase, the subjects got an [additional printed handout](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/handouts/tools.pdf) that contained a one page brief summary about the features as a reminder.

### Categorization of the Behaviors

The preprocessing phase started with the manual inspection of the collected data: we watched the videos and determined the aspects and categories based on the witnessed behavior.
In the next step we systematically watched all the recordings again, and assigned the appropriate categories to each parts of the experiment.
The aspects and categories were described in the respective publications.

We exported the list of [categories](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/preprocessing/macros.csv) and the actual [categorization](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/preprocessing/categorization.csv) for the 6 participants as CSV files.

### Graphs of Categorization

The transition between categories, i.e. how the participant behaviour moves from category to category between phases of experiment are published as [graphs](https://github.com/search?q=repo%3AInteractiveFaultLocalization%2Fthink-aloud-utils+extension%3Agraphml+path%3A%2Fpreprocessing%2F&type=Code&ref=advsearch&l=&l=).
The format of these files are [GRAPHML](http://graphml.graphdrawing.org/), and we included all the original data as properties for edges and nodes.
We used the [NetworkX](https://networkx.org/) Python library to generate these files and we recommend [yEd](https://www.yworks.com/products/yed) graph editor to display them.
Also, the [property mapper](https://yed.yworks.com/support/manual/properties_mapper.html) can be used and after that the [BPMN layout](https://yed.yworks.com/support/manual/layout_bpmn.html) feature of yEd to display these graphs in a more user-friendly way. We also provide a [sample mapping](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/preprocessing/ifl.cnfx) for the properties. Please remember to apply both of the two mappings placed in this file: edge and node mapping.

We also created a [preformatted PDF version of the full transition graph](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/preprocessing/arcs_full.pdf) for your convince.

### Categorization Preprocessing Script

The inner structure of these datafiles can be inferred from the Python [script](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/preprocessing/main.py) used to generate them.

## Raw Data from Simulated Users Experiments and User Studies in 2020

In 2020, we conducted several experiments using simulated and real users.
The collected raw data are available under the following sections. For more details check our publications.

### Collected data

The data collected ([Zenodo](https://doi.org/10.5281/zenodo.4658314), [Figshare](https://doi.org/10.6084/m9.figshare.c.5099597.v2)) from these experiments are presented in several CSV files. These are grouped according the type of the experiment: simulation and user-study.
We also provide the exact bugs as patches in those cases when we did not use any official bug databases.

### Environment

This is the [development environment](https://figshare.com/articles/software/Software_for_Experiments_with_Interactive_Fault_Localization_Using_Simulated_and_Real_Users/12845921?backTo=/collections/Supplemental_Material_for_Experiments_with_Interactive_Fault_Localization_Using_Simulated_and_Real_Users/5099597) which was used during the evaluation of the iFL4Eclipse plug-in.
