---
layout: post
title: Rethinking Awesome Lists
---

Start with Stuffs look Irrevelant
-------------------------------------

Programming is a dramatically huge world. Given one small topic like *matching
algorithm*, you can find tons of results that'll take you years to master all.
Let me give you some concrete examples to deeply understand what I mean:

1. You have $$M$$ workers and $$N$$ missions. (Yes, the starting point of each
boring algorithm problem.) Different worker masters different mission,
differnet mission costs you different money. Try to come up with an algorithm
that can maximize the worker-mission assigment efficiency and minimize the cost
at the same time.

    This is called the *assignment problem* or the *matching problem*. You need to 
    match units from two groups. The matching can only be one-to-one, and, you
    have some metric/number that stands for the performance of your matching.

    DO NOT exploit one single worker because he/she masters everything and let
    other worker be ilde like they are waiting for mom's breastfeeding (in some
    domain, this situation is called *MANAGER*). That's the real world, we are
    now in the Ivory Tower of programming.

2. You are developing an anchor-based object detection deep learning model. The
model will output tons of rectangles in one single image (e.g. 25,200). The
ground truth label only consists of 10 rectangles in the same image. Now you
need to match these 25,200 rectangles with the 10 ground truth rectangles,
otherwise, you are unable to compute the loss.

    This is also another *matching problem*. The units in this case are
    bounding boxes, $$M$ is 25,200, $$N$ is 10, and, two groups become model
    output and ground truth label. The previous example told you the costs
    beforehand, but what are the costs for this case? To leverage the matching
    algorithm, you need to learn *the costs of bounding boxes* first. So you
    google them, you find IoU, Intersection over Union, it's a simple formula,
    easy to learn and implement in 10 minutes. Your model start training, you
    are now in the world of AI.

    Then you wake up from the movie dream.

    Life kicks your ass right after this. How come your matching result looks
    garbadge? By means of garbadge, you refer to the visualization of the matching
    results, not the speed, because we are in modern programming, PYTHON. You check
    every shitty code's details, they are all correctly implemented. So, why? You
    eventually know it's the limitation of IoU, now you need to learn improved IoU
    to let your matching algorithm works. Guess what? DIoU, GIoU, CIoU, EIoU,
    Alpha-IoU, etc.

    You look at the calendar, 2 months passed, you just want to learn and implement
    a matching algorithm in the beginning.


Now come back to my first statements. Programming is a dramatically huge
world. No domain exists like an isolated island. Each topics overlap, the world
looks like huge bubbles are merging with each other, and, sometimes another
bubble emerge from nowhere and you don't know why.


Awesome Lists
-------------

People always feel deeply anxious when facing any huge world like programming.
To mitigate, we intuitively hope we can understand how this world looked like in
a high level(Yes, the idiot's high level decision reasoning.), and we can plan well
based on this high level understanding.

Introducing Awesome Lists, a novel, modern, user friendly, fancy, eco-friendly,
blazingly fast improvement, politically alwyas correct, contridution welcomed,
500GB README.md file. This list curates all you need to improved in the
*matching problem* world. Please refer to the table of contents to know the
whole pace.

Did you notice you just read through an useless paragraph? Try to recap how much
this shitty paragraph you met when googling. They exist everywhere, Medium, FOSS,
RealPython, GeeksforGeeks, etc. They leverage the knowledge chain to extend their
article length, levave the reader being exhausted beofre actually read the core
content, let them need to go back another day to literally start learning.

Go back to the github awesome list repo. You see a small, tiny scroll bar. You
look at the amount of stars, 15.2k, you think everyone like this, this should
be good. You feel content, your learning pace will start tomorrow, you have a
bright future.




Conclusions
-----------
