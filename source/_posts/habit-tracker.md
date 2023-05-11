---
title: How to Build a Habit Tracker in Roam Research
cover_index: /assets/habit-tracker.png
date: 2021-01-09 14:44:53
tags:
---

For the past 2 years, I've been tracking my habits as a low effort way to maintain my daily and weekly commitments for my health, relationships and work. Every month or so, I re-evaluate the habits I'm tracking and update the habit tracker accordingly (more on this and the pitfalls of habit tracking later).

Previously I have been tracking these in Evernote, sub-optimally. But with the arrival of the new year and the introduction of `[[roam/templates]]`, I  have finally moved my habit tracker to [Roam Research](https://roamresearch.com/).

<h1 style="font-size: 1.6em;">Here's how to set it up</h1>

1. Create a `[[roam/templates]]` page if you don't already use Roam templates.
2. Pick a name for the habit tracker, this will be your template label. I use the un-imaginative label Habit Tracker.
3. Follow the following format (the correct indentation is important)

<img src="/habit-tracker/format.png"
    style="width: 100%;
    display: block;
    margin: auto;"
    alt="">
</img>

You can copy it here.

```
Habit Tracker #[[roam/templates]]
  - [[habit tracker]] [[Jan 2021]] 
    - {{[[TODO]]}} [[habit: walk]]
    - {{[[TODO]]}} [[habit: write]]
```

4. Each day, you can load the template on the daily page by typing `;;`. I'm hoping that eventually we'll be able to pre-populate the daily pages with a specific template without having to do it manually.

<img src="/habit-tracker/fetch.png"
    style="width: 100%;
    display: block;
    margin: auto;"
    alt="">
</img>

5. During your review process, you can measure each habit by running the following query:

```
  {{[[query]]: {and: [[habit tracker]] [[DONE]] [[habit: walk]]}}}
```

<img src="/habit-tracker/query.png"
    style="width: 100%;
    display: block;
    margin: auto;"
    alt="">
</img>


That's all on creating a habit tracker in Roam. However, I'd like to add a few words on the broader concepts of habit tracking and goal setting.

<h1 style="font-size: 1.6em;">The pitfalls of habit tracking</h1>

While it's helpful to have a habit tracking system, It's important to address some of the pitfalls we fall into when tracking our habits. 

Sometimes the habits we choose to develop and track aren't driven from the right place. We pick habits that we think we **should** develop. We are inspired by the prospects of those habits without taking into account how those habits will actually fit into our day. Even if we can fit them into our day, we often fall off the habits wagon after some time.

Instead, we need to **take a step back and evaluate what we want out of our life.** Where do we want to go in life and why do we want to go there?

Once we choose a goal or a habit from a deep place of "why", it becomes easy to maintain. We can try each habit for a month and then re-valuate it for the following month. This way we can let our introspection and our real-life experience direct us.

I've created a guide called [The Power of Knowing What You Want](https://gumroad.com/l/pkwyw) that walks you through this process and many others in more detail. Currently, it's a Notion dashboard 🙈 but I plan to create a Roam version in the future.

<a href="https://gumroad.com/l/pkwyw">
  <img src="/assets/pkwyw-cta-round.png"
      style="width: 100%;
      display: block;
      margin: auto;"
      alt="">
  </img>
</a>

---

Thanks for reading. If you enjoyed this post, you may also like [how to make the most out of online course in Roam](/roam).
