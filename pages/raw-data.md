---
title: "Replication Packages"
---

## Sample Projects for Hands-on Session at A-Test Workshop in 2022

The following packages contain a single version of the subject system seeded with at least one real-life error. Please check the official project pages for details about how to build, execute, and use the tools.

|| name | system |
|:--:|--|--|
| ![java](/pages/logo/java.svg){: .charsize} | [lang-3](/pages/data/lang-3.zip) | [Commons Lang](https://commons.apache.org/proper/commons-lang/) |
| ![java](/pages/logo/java.svg){: .charsize} | [lang-7](/pages/data/lang-7.zip) | [Commons Lang](https://commons.apache.org/proper/commons-lang/) |
| ![java](/pages/logo/java.svg){: .charsize} | [lang-22](/pages/data/lang-22.zip) | [Commons Lang](https://commons.apache.org/proper/commons-lang/) |
| ![java](/pages/logo/java.svg){: .charsize} | [lang-50](/pages/data/lang-50.zip) | [Commons Lang](https://commons.apache.org/proper/commons-lang/) |
| ![java](/pages/logo/java.svg){: .charsize} | [lang-55](/pages/data/lang-55.zip) | [Commons Lang](https://commons.apache.org/proper/commons-lang/) |
| ![java](/pages/logo/java.svg){: .charsize} | [lang-61](/pages/data/lang-61.zip) | [Commons Lang](https://commons.apache.org/proper/commons-lang/) |
| ![python](/pages/logo/python.svg){: .charsize} | [black-10](/pages/data/black-10.zip) | [Black - The uncompromising code formatter](https://commons.apache.org/proper/commons-lang/) |
| ![python](/pages/logo/python.svg){: .charsize} | [black-20](/pages/data/black-20.zip) | [Black - The uncompromising code formatter](https://commons.apache.org/proper/commons-lang/) |

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
The participant starts the exercise. He says 'well I'm gonna run the base...' he looks down at the instructions 'or... next to the green run button from the arrow pointing down we choose the TaskA configuration from the dropdown menu.'<br/>
He double checks the task, sighs, and repeats it while finding the appropriate menu. 'From the dropdown menu choose... okay.'<br/>
He clicks on the TaskA test and runs it.<br/>
He makes observations while waiting. 'Now I'm waiting for it to finish running. I can see this is a Maven project, though I could guess that from the src/main/java structure and from the POM.'<br/>
'It's interesting though, because the JRE system library says Java 1.6, but here it was run with 1.7' he adds, then clears his throat.<br/>
'Well anyway, I'll look into this' he says before looking up to see the finished test.<br/>
Looking at the Console log he continues. 'Okay here I can see... it deleted them.'<br/>
He pauses for a moment to adjusts his glasses.<br/>
'I'll search for... in math the... erm NumberUtils.java' he says while clicking the folders in the Project Explorer.<br/>
He opens the file he was looking for and continues. 'But otherwise you should search for it in the test, but for this Java class (unintelligible)... you can make sense of the test.'<br/>
He starts opening other files from the Explorer while adding 'I will open these and I'll search for the testCreatNumber test.'<br/>
He seems to have difficulty finding the test, however, and mumbles 'This is a constructor... testToInt... string...' then decides to change tactics.<br/>
'This is a relatively long file so I will search with CTRL+F.'<br/>
He opens the Find/Replace window.<br/>
'Umm... I hope this will work.'<br/>
'I'm looking for the testCreat' he explains while typing it into the window, 'but anyway in Eclipse there should be an option to see the functions...' He starts looking for the settings.<br/>
'In Window, maybe Editor... Show view, and here is one called... not Project, buuut... Expressions maybe?' He clicks it. It's not the one he wanted.<br/>
'Nope nope nope nope' he realizes, and clicks away to continue looking elsewhere.<br/>
'I want to see somewhere the... what this contains' he goes on, but decides to give up for fear of losing too much time.<br/>
'Never mind, I'll just search for it instead of wasting more time on it, because I don't know how they planned this one and a half hour.'"
%}

{% include collapse.html title="Transcript of debugging session with additional tools (2021-02-24_13-40-45-ENG, sample)"
content="
'Oookay, now let's see... what's going on here'<br/>
The participant starts the task by clicking on the test case.<br/>
While it loads he thinks aloud about his next steps. 'Well I don't know; I don't think coverage can help us much right now.' He scratches his head. 'I'm not trying to write a new test. Well okay, clearly we can look at what it shows...' he stops as he only sees an empty table under Coverage, 'oh, yeah especially if... If this is not how you do it at all...' he muses, 'but by default did it not...?'<br/>
He comes to a realization.<br/>
'It didn't run, well never mind then. Well then what to do, what does it say...' He sighs deeply while looking down at the task description.<br/>
'Yes, coverage as, [click] on coverage all, on coverage all.' He figures out what to do.<br/>
'Good, click JUnit test, mhm' he muses while clicking in the menu.<br/>
He then looks down at the task description again.<br/>
'Call graph... it's super interesting though, that Atlas plugin. It's possible it won't be able to help in this exact situation, I'll look into it in a second...'"
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
'So I will lower this, I won't modify the others yet, but I'll lower this, 'cause this definitely won't have errors.'<br/>
'Getter' he says and continues clicking.<br/>
He finds an issue he's not happy with. <br/>
'Mutable ... oh yes, here with the ordering - I would report a bug with iFL that if you modify the context, then the ordering will disappear.' Then he keeps searching. 'Denominator... erm... I could do multiple ones at the same time' he muses about checking the result items. 'Erm Fraction, here well, I suppose there won't be any errors here either' he says and moves on. 'Erm... getReduceFraction... here the rows are a little skewed, Position, but whatever, I found these, this is fine.'"
%}

{% include collapse.html title="Discussion about the hypothetical cases (2021-02-24_12-28-37-ENG, sample)"
content="
The participant is asked about hypothetical situations and his reactions to them. The instructor has the following question:<br/>
'Okay, then let's see the next such case. Let's say that during the task you solved last time, when you wanted to examine the errors within the project, loading the list would have taken 5 minutes meanwhile the Eclipse development environment wouldn't respond to commands. How would this have affected you?'<br/>
'Well, uuuh,' begins the participant. 'I had such a, well not exactly this issue, but... I had library problems. For me it explicitly underlined the... I think the StringUtils, and uuuh, when you have a specific task, then those errors that do not belong there can be really annoying' he chuckles and goes on. 'And then others also come out... obviously a project clean and etc. can solve this, usually, in Eclipse. But otherwise, yeah, it annoys me a little.' He pauses to adjust his mask and continues. <br/>
'Or if there are those that, well, that are quite unexpected... that for completely separate reasons, just a kind of fiddling around, like let's say the development environment is how it is, or the... the development tool, or the computer, or the whatever else, then that can annoy me quite a lot.'<br/>
There is a hum of approval from the instructor. <br/>
'I'm not saying it would specifically negatively affect it, because this usually does occur, so it is a typical developer error... So it's not that negative, rather it just causes stressful situations, especially if you have a deadline' he emphasizes. 'And here I imagine this as a deadline, because time... there is a time limit during which you should be finished, and my expectation is that I want to be able to finish' he elaborates.<br/>
The instructor again acknowledges the answer with a hum, and the participant is spurred on to give further information. <br/>
'It might just be because of this, or if somebody... I'm sure there are people to whom... to whom it doesn't matter, because they don't care about it. To me this is more like a competition, this situation a bit, and so I want to do it well, and then every other such thing bothers me' he explains, laughing a little. <br/>
'So this is how it affects me, it's like it like creates a stressful situation... yeah' he concludes."
%}

{% include collapse.html title="Discussion about the hypothetical cases (2021-02-26_12-41-18-ENG, sample)"
content="
The participant is asked about a hypothetical situation and his potential reaction to it.<br/>
The instructor introduces the situation.<br/>
'So, our first case is no. 17075, and it goes like...' he pauses because an ambulance is passing outside the window. 'like WEE-oww,' he jokes. 'Let's wait this out.'<br/>
Once the sirens are more distant he continues.<br/>
'Alright, so 17075, the methods are in a descending order based on score in the iFL tool, and you can find the createNumber method in 7th place in this list that is in a des... descending order based on score. So it's on the first page, it's the penultimate out of the 8 cards.'<br/>
'The last one, yeah' affirms the participant (incorrectly).<br/>
'Uuuuh, let's say that this is the method with the error, so before this one you already had to examine 6 other methods... erm, there were some here like... it's one of the bugs from Monday, I don't know how well you remember it, it was full of these create... methods, createFloat, createBiginteger, and...'<br/>
'Yes-yes' interjects the participant.<br/>
'... nonessestial stuff like that. BigDecimal and whatnot.'<br/>
'Yes-yes.'<br/>
'So this is the situation that there is this page full of methods in iFL, the 7th is the... the penultimate is the... the createNumber, of which we later learn that it is the one with the error, but you don't know that yet uuh, and by the time you get there, now let's assume that you insist... well maybe not insist, but you use iFL's list to help you, and you already had to examine six methods, by the time you finally end up with the one that has the errors.'<br/>
The participant thinks for a bit before asking.<br/>
'Erm, and so... What is the question?' he laughs. 'Yeah, I know, there is no question... well erm...'<br/>
The instructor adds 'Well basically... what is your opinion about the situation, does it affect you-'<br/>
'I see.'<br/>
'...in any way...?'<br/>
'Well the problem is that... I didn't exactly understand, or like... I don't know if I should have understood, what, what this tool... erm, what it does, or rather how does it do... well how much, uuh can you, uuh rely on it, so...'<br/>
'If it's important to you, then I can tell you how those lists come to be' suggests the instructor.<br/>
'Well, uuuuuh... yeah' admits the participant after some hesitation.<br/>
'So this is a... this technique is called spectrum-based fault localization, where the spectrum and the coverage-'<br/>
'Mhm'<br/>
'... well technically the spectrum is the coverage. There's only one twist in the whole thing, namely that we are not looking at how you run the test suite and so what that covers, but instead for each test you determine the... what they cover, so what methods... and from this you'll have a freaking huge matrix. And we also have which methods, or I mean which tests ran with what results; whether they passed or failed. Erm, and then you can get all sorts of interesting statistics from this. There are thousands of millions of formulas for how you eventually calculate the score from this amount of data, but the basic assumption is that the most suspicious, so the method with the highest score... erm, is the one on which only failing tests pass. So you run the failing test and what that touches on is suspicious.'<br/>
'Yes.'<br/>
'You can add nuance to this by also running passed tests, and they also touch on the ones that the failing ones did too, then there it drops a bit, so it's different...'<br/>
'Mhm, so there are tests that pass and is included in them, mhm.'<br/>
'And it includes what the failing did as well... sooo let's say you have three methods, A, B, and C; these are covered by the failing one, and you have two other tests that also touch on B and C and they passed' elaborates the instructor. The participant follows along, often nods and hums in understanding. 'Then the assumption is that A is more suspicious than B or C because that one was only included in the failing test. Then there really are thousands of millions of formulas to precisely take advantage or to calculate this... Uuuuh, and then these result in a score, usually between 0-1, uh, and then that makes the list.'<br/>
'Mhm, and that csv, that scores... is that... that... how does that connect to this, is that the output of some...' questions the participants unsurely.<br/>
'Yes it connects to this by... Yes, so this is a pretty slow and lengthy measurement process by the time these scores are produced, because it's freaking huge...'<br/>
'Ah, so it's calculated beforehand and then this is the result.'<br/>
'And then this is the result.' affirms the instructor.<br/>
'Ah, I see... mhm...' the participant starts thinking again with the new information in mind.<br/>
'Do you want me to read the situation again?' asks the instructor.<br/>
The participant thinks for a second, shakes his head and starts his answer.<br/>
'Uuuuh, no you don't have to, so the point is that... that our affected method is relatively... it's in the penultimate position in the top...'<br/>
'Eight, yeah' amends the instructor.<br/>
'Top eight, mhm.'<br/>
'Well whether it's the penultimate or not...'<br/>
'Yeah yeah, it's at the end, yeah' agrees the participant and takes some time to gather his thoughts.<br/>
'So for this, in this case you can... well obviously, if I know that... that that is the method that interests me... but then I clearly already got there, like let's say I looked at the first one or the ones before it and then I could use that tool to set the score... uuuuh ratios, or?' he asks, unsure.<br/>
'With percentages, you can decrease or increase...'<br/>
'Okay, then I could pretty much do that. I would either increase its score compared to the others'... compared to the ones before or... or I could lower the score of the previous ones'?'<br/>
'Exactly.'<br/>
'And by the way is that only for... only good for... let's say pulling my, or the affected method forward?'<br/>
'Yyyyyes, yeah-yeah' confirms the instructor (unconvincingly) after some hesitation.<br/>
'But so this is not for some kind of training... this is just for the given display...'<br/>
'This is just static, yeah-yeah.' They both start talking at the same time, but the floor is given back to the instructor to continue. 'It's an interesting aspect, I'm gonna jot that down' he jokes and they both laugh. 'That uuuuh...'<br/>
'So this is just about like... like get these out of here, I don't care about them, but let's say, bring those forward that are more interesting to me' suggests the participant. They still keep talking over each other a bit.<br/>
'Obviously you don't know from the get go what you'll find.'<br/>
'Yeah, you just make those disappear that... mhm, that are no longer... mhm'<br/>
'... you can weigh them, or even completely rule them out, and then the others come forward' explains the instructor.<br/>
The participant goes on to give this more thought."
%}

### Handouts

At the beginning of each debugging session we gave printed handouts [HU](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/handouts/tasks.pdf), [EN](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/handouts/task_en.pdf) to the participants which contained the following information:

+ ID of the task (A, B, etc.)
+ Failing test case(s)
+ Short description (one sentence) of the failure
+ Execution instruction about the test suite

Before warm-up and debugging session of the feature phase we provided further information about the main features of the three IDE plug-ins, which were introduced during this phase.
At the beginning of the debugging sessions in the feature phase and use-case phase, the subjects got an additional printed handout [HU](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/handouts/tools.pdf), [EN](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/handouts/tools_en.pdf) that contained a one page brief summary about the features as a reminder.

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
