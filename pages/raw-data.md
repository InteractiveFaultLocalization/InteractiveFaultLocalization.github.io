---
title: "Additional materials"
---
## Raw Data from the Think Aloud Protocols in 2021

In 2021, we conducted an experiment with 6 developer using the [Think Aloud Protocol](https://psycnet.apa.org/record/1980-24435-001). The collected raw data are available under the following sections. For more details check our publications.

### Transcription of the Videos

We obtained video material of total length of 33 hours and 57 minutes.
Each video frame was composed of two parts: the participants screen area and video footage.
We created a transcription of each recorded video in form of subtitles (SRT format) with additional information about gestures and other activities of the participants such as relevant changes of facial expression, gesticulation, and other environment factors (this is similar to subtitles for the deaf and hard of hearing for movies).
After this step, all the videos could be edited to remove identifying information, that is video and voice of the participant, and leave only the screen capture part with the transcript.

You could download the transcripts [here](https://github.com/InteractiveFaultLocalization/think-aloud-utils/tree/iFL2021/video-logs).

### Categorization of the Behaviors

The preprocessing phase started with the manual inspection of the collected data: we watched the videos and determined the aspects and categories based on the witnessed behavior.
In the next step we systematically watched all the recordings again, and assigned the appropriate categories to each parts of the experiment.
The aspects and categories were described in the respective publications.

We exported the list of [categories](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/preprocessing/macros.csv) and the actual [categorization](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/preprocessing/categorization.csv) for the 6 participants as CSV files.

### Graphs of Categorization

The transition between categories, i.e. how the participant behaviour moves from category to category between phases of experiment are published as [graphs](https://github.com/search?q=repo%3AInteractiveFaultLocalization%2Fthink-aloud-utils+extension%3Agraphml+path%3A%2Fpreprocessing%2F&type=Code&ref=advsearch&l=&l=).
The format of these files are [GRAPHML](http://graphml.graphdrawing.org/), and we included all the original data as properties for edges and nodes.
We used the [NetworkX](https://networkx.org/) Python library to generate these files and recommend [yEd](https://www.yworks.com/products/yed) graph editor to display them.
You could use the [property mapper](https://yed.yworks.com/support/manual/properties_mapper.html) and after that the [BPMN layout](https://yed.yworks.com/support/manual/layout_bpmn.html) feature of yEd to display these graphs in a more user-friendly way. We also provide a [sample mapping](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/preprocessing/ifl.cnfx) for the properties. Please remember to apply both of the two mapping placed in this file: edge and node mapping.

We also created a [preformatted PDF version of the full transition graph](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/preprocessing/arcs_full.pdf) for your convince.

### Categorization Preprocessing Script

The inner structure of these datafiles can be inferred from the Python [script](https://github.com/InteractiveFaultLocalization/think-aloud-utils/blob/iFL2021/preprocessing/main.py) used to generate them.