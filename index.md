---
title: "Home"
---
## Introduction

{% include left-img.html img="mascot/dev_with-hammer.png" img-width="30%"
content="He is a software engineer, who create various software system for several, different users. But his daily workflow does not contain writing the source code but ensuring that it is working correctly. To that end, he usually creates some unit tests to check the functionality of his code. If any of these tests fail, it means that there is an error either in the production or the test code." %}

{% include center-img.html img="mascot/bugs.png" img-width="30%"
content="And these are the bugs, the mistakes, which prevent the software from accomplishing its tasks correctly. They could be present all over the system, and sometimes they are tough to spot and fix." %}

{% include left-img.html img="mascot/inspect.png" img-width="20%"
content="The developers usually have to check several code elements, like packages, classes, and methods, until they find the \"buggy\" ones. During this process, which is usually called fault localization, they use various debugging techniques and tools to speed up their work. For example, they manually inspect the related code chunks, or they modify to make the error more prominent, hence easier to catch. There are various debugging tools, which allowed to examine the states of the software during execution." %}

{% include center-img.html img="mascot/rank.png" img-width="30%"
content="Our research key concept is another kind of fault localization technique. It analyzed the tests' results and used the list of code elements that are executed during the testing to compute a score for each part of the code. They are the Spectrum Based Fault Localization methodologies (or SBFL) for short. The score usually expresses the suspiciousness of the code elements. For example, when a method got a higher score, it is more likely that the developer will find the bugs in that particular method." %}

{% include right-img.html img="mascot/dev_think_right.png" img-width="30%"
content="But these algorithms and their formulas (which they have quite a few!) are not perfect. So the developer thinks that there are several parts of the code which he knows to be correct, right? For example, trivial `getter` and `setter`, classes he already checked, etc. Sure some methods seem suspicious, but can not we get rid of the clutter?" %}

{% include left-img.html img="mascot/alg_ranks_left.png" img-width="40%"
content="To answer these questions we created a new methodology, called Interactive Fault Localization (iFL, for short), where the ranked list of suspicious code elements are a result of the discourse between the algorithm and the developer. Our idea was that we let the user modify the score of the methods, classes, etc., by giving various feedbacks about the suggested items. This way, both of them could concentrate on the task they excel in. The algorithm collects and analysis test results and test-code coverage data, while the developer could use his expert knowledge about the system to clean up the list of suspicious items. Finally, we continue to improve the iFL methodology and its implementations to find the bugs faster." %}

{% include center-img.html img="logo/logo.png" img-width="40%"
content="For more information about the technical details of iFL and the current state of the research, you could check our previous publications." %}

## Name our Little Friends!

<div style="text-align: center">
    <a href="https://forms.gle/eTGFVMDtrA6KprMT7"><img src="mascot/alg_sign.png" style="width: 40%; display: inline"/>
    <img src="mascot/dev_sign.png" style="width: 25%; display: inline"/></a>
</div>

You could suggest a name for the developer and for the robot by filling this [anonymous form](https://forms.gle/eTGFVMDtrA6KprMT7).
