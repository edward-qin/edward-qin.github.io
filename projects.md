---
layout: page
title: "Projects"
permalink: /projects
---

- [Systems](#systems)
  - [Distributed Systems Paper Replication (Work in Progress)](#distributed-systems-paper-replication-work-in-progress)
  - [Distributed Key-Value Store and Other Course Projects](#distributed-key-value-store-and-other-course-projects)
- [Web Projects](#web-projects)
  - [IDIOT Game](#idiot-game)
  - [Daily Tab Opener Browser Extension](#daily-tab-opener-browser-extension)
  - [PhotoFilter App](#photofilter-app)
- [Machine Learning](#machine-learning)
  - [Multi-Pitch Estimation](#multi-pitch-estimation)
  - [Math Word Problems](#math-word-problems)
  - [Machine Learning Optimizers](#machine-learning-optimizers)
  - [Jappanese Art DCGAN](#jappanese-art-dcgan)

Below is a showcase of some projects I have worked on.

## Systems

### Distributed Systems Paper Replication (Work in Progress)

I am currently exploring more in this area.

### Distributed Key-Value Store and Other Course Projects

For a distributed systems course, I worked with a partner to implement a distributed key-value store that was linearizable, fault-tolerant, dynamically sharded, and supported multi-key cross-shard transactions. The course project also incorporated protocols like 2-Phase Commit and MultiPaxos. This was a valuable learning experience where I learned to think of and write clear design docs. Design was essential to correctness, and I also had to really learn to use logging and debugging tools to make up for places where our design lacked.

Note that there is no link to the project since this was course project and lives in a private repository because UW's course projects are reused across different quarters. However, other meaningful course projects of mention that I have completed include a MiniJava compiler, flight transactions database, and C/C++ web/file search index.

## Web Projects

### IDIOT Game

The game is playable here: [IDIOT Game](https://edward-qin.github.io/Idiot-Game/){:target="_blank"}

This is my favorite word game. It is fast to learn, and only requires your brain and a group of friends. The premise is to try not to complete a word, but rather make another player complete a word. More instructions are provided in the physical game linked above. I wanted to implement this project to help improve solo practice and accessibility to the game. This was also a great chance to practice my design and basic front-end skills.

### Daily Tab Opener Browser Extension

The extension is available for Firefox here: [Daily Tab Opener](https://addons.mozilla.org/en-US/firefox/addon/daily-url-opener/){:target="_blank"}

During one school break, I felt the need to motivate myself. I found that I was unmotivated to practice Leetcode interview problems. I had also been wanting to read the daily xkcd comic. As such, I figured it would be a smart idea to make a tool that could open the daily comic webpage and daily Leetcode problem. As a result, this was a self-contained, one-week project where I learned the basics of browser extensions and published the extension in the Firefox Add-Ons store.

### PhotoFilter App

The relevant github repository lives here: [PhotoFilter App](https://github.com/edward-qin/PhotoFilter){:target="_blank"}

Over a couple months, a friend and I wanted to build a mobile app that can filter photos. In the process, we learned about kernels and basic image pixel manipulation techniques. This was a full-stack project where we used the [React Native](https://reactnative.dev/){:target="_blank"} framework in the frontend and the [SparkJava](https://sparkjava.com/){:target="_blank"} framework for the server. This experience also taught us a lot about unblocking issues as we explored new frameworks by getting our hands dirty with debugging and consulting documentation.


## Machine Learning

### Multi-Pitch Estimation

The paper can be found here: [Multi-Pitch Estimation](/assets/multi_pitch_estimation.pdf){:target="_blank"}

For the final project of a machine learning for music course, I worked with a group to evaluate multi-pitch estimation. The course was pilot course meant to explore machine learning applied in music. One of the largest problems in ML for music involves pitch estimation, especially when there are multiple pitches. This is a difficult problem because harmonics and the underlying physics behind sound waves can cause one pitch to be interpreted as another pitch. Our project highlights the importance of data augmentation by adding noise to synthetic, clean audio samples during training. Additionally, augmenting training with combined datasets of chords, intervals, and single notes imporves generalizability.

### Math Word Problems

The paper can be found here: [Math Word Problems](/assets/math_word_problems.pdf){:target="_blank"}

For the final project of a natural language processing course, I worked with a group to evaluate cooperative reasoning for math problems. LLMs traditionally perform poorly on math problems, and this field is thus a challenging direction to explore. We evaluate the paper on varying sized GPT-based models, providing an analysis on performance on smaller models and of the generator and verifier models in cooperative reasoning.

### Machine Learning Optimizers

The paper can be found here: [Machine Learning Optimizer](/assets/optimizers.pdf){:target="_blank"}

For the final project of a machine learning course, I worked with a group to survey the history of optimizers. For the first half of the course, we had covered some learning theory including Empirical Risk Minimization, VC Dimension, and Rademacher Complexity, as well as how SGD and Adam optimizers work. We hoped to delve deeper into understanding the theory behind the many optimizers used in machine learning research, thus producing this paper.

### Jappanese Art DCGAN

The site discussing the project can be found here: [Japanese Art DCGAN](https://edward-qin.github.io/Japanese-Art-DCGAN/){:target="_blank"}

For the final project of a computer vision course, I worked with a partner to train a Deep Convolutional Generative Adversarial Network for Japanese Art. Using 64x64 pixel images from the [WikiArt Art Movement/Styles](https://www.kaggle.com/datasets/sivarazadi/wikiart-art-movementsstyles){:target="_blank"} dataset, we were able to produce images that matched the Japanese Art style from the era, but lacked distinct features that defined exact objects. This was largely due to our incorrect approach of not training over iterations of incrementing image sizes (i.e. from 16x16, then 32x32, and finally 64x64), and our still relatively small image size. However, this was a rewarding experience in both learning about the GAN model and gaining hands-on experience with training computer vision models.
