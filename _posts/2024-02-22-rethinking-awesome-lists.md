---
layout: post
title: Rethinking Awesome Lists
---

TL;DR
-----
Popular awesome lists can be easily found by google once, so you don't need to
keep it existing in your tabs. You even don't need to follow the order it
offers to learn. Use it as a dictionary. Keep looking at the long list is quite
harmful and has no benefit to you.


Start with Stuffs look Irrelevant
---------------------------------

Programming is a dramatically huge world. Given one small topic like *matching
algorithm*, you can find tons of results that will take you years to master all.
Let me give you some concrete examples to deeply understand what I mean:

1. You have $$M$$ workers and $$N$$ missions. (Yes, the starting point of each
boring algorithm problem.) Different worker masters different mission,
different mission costs you different money. Try to come up with an algorithm
that can maximize the worker-mission assignment efficiency and minimize the cost
at the same time.

    This is called the *assignment problem* or the *matching problem*. You need
    to match units from two groups. The matching can only be one-to-one, and,
    you have some metric/number that stands for the performance of your
    matching.

    DO NOT exploit one single worker because he/she masters everything and let
    other worker be idle like they are waiting for mom's breastfeeding (in some
    domain, this situation is called *MANAGER*). That's the real world, we are
    now in the Ivory Tower of programming.

2. You are developing an anchor-based object detection deep learning model. The
model will output tons of rectangles (e.g. 25,200) in one single image. The
ground truth label only consists of 10 rectangles in the same image. Now you
need to match these 25,200 rectangles with the 10 ground truth rectangles,
otherwise, you are unable to compute the loss.

    This is also another *matching problem*. The units in this case are
    bounding boxes, $$M$$ is 25,200, $$N$$ is 10, and, two groups become model
    output and ground truth label. 25,200 x 10 is a huge $$n$$ for any matching
    algorithm. So you need to filter the 25,200 boxes first. Here comes the
    NMS, Non-Maximum Suppression, an algorithm to pick out the boxes by
    progressively delete similar ones until the remaining ones are not similar
    enough. You need a metric to define the similarity, so you google them, you
    find IoU, Intersection over Union, it's a simple formula, easy to learn and
    implement in 10 minutes. Your NMS algorithm works, good.

    Now your problem becomes matching between 100 boxes and 10 boxes. The
    previous example told you the costs beforehand, but what are the costs for
    this case? To leverage the matching algorithm, you need to learn *the costs
    of bounding boxes* first. You leverage IoU again and the model starts
    training, you are now in the world of AI, awesome.

    Then you wake up from the movie dream.

    Life kicks your ass right after this. How come your matching result looks
    garbage? By means of garbage, you refer to the visualization of the
    matching results, not the speed, because we are in modern programming,
    PYTHON. You check every shitty code's details, they are all correctly
    implemented. So, why? You eventually know it's the limitation of IoU, now
    you need to learn improved IoU to let your matching algorithm works. Guess
    what? DIoU, GIoU, CIoU, EIoU, Alpha-IoU, etc.

    You look at the calendar, 2 months passed, you just want to learn and
    implement a matching algorithm in the beginning.


Now come back to my first statements. Programming is a dramatically huge world.
No domain exists like an isolated island. Each topics overlap, the world looks
more like a huge collection of bubbles, each of them are slowly merging with each
other, and, sometimes another bubble emerges from nowhere and you don't know
why.

Awesome Lists
-------------

People always feel deeply anxious when facing a huge world like programming. To
mitigate, we intuitively hope we can understand how this world looked like in a
high level view (Yes, the idiot's high level decision reasoning.), and we can
plan well based on this high level understanding.

Introducing Awesome Lists, a novel, modern, user friendly, fancy, Eco-friendly,
blazingly fast improves, progressively grows, politically always correct,
contribution welcomed, 500GB README.md file. This list curates all you need to
improve in the *matching problem* world. Please refer to the table of contents
to know the whole pace. GLASSES EMOJI

Did you notice you just read through an useless paragraph? Try to recap how
many those shitty paragraphs you met when googling. They leverage the knowledge
chain (or, bubbles) to extend their article length, leave the reader being
exhausted before actually read the core contents, let them need to go back
another day to literally start learning.

Go back to the github awesome list repo. You feel exhausted after reading the
long introduction paragraph. You see a small, tiny scroll bar. You look at the
amount of stars, 15.2k, you think everyone like this, this should be good. You
feel content, your learning pace will start tomorrow, you have a bright future.

Tomorrow morning, you wake up, you open the repo in your browser. Tons of good
resources out there. You click them all, skim through each one, try to pick one
that best suited your needs. You write a notion page to summarize all of them,
help yourself being more productive on being productive. 4 hours later,
you finished the notion list. Each page are classified well, you pick your best
one. You are glad. Let's start learning tomorrow.

You'll find yourself repeat this process again and again. You just keep finding
the best one and never start learning. Until you realize the problem, 6 months
passed. You look at the list again, lots of pressure and disappointed from the
bottom of your heart.

The only way to get rid of this situation is just start building, recreating
more and more wheels as you can, period. Avoid those lists, focus on learning,
not collecting.
