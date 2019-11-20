---
layout: page
title: Projects
permalink: /projects/
---

## Current Projects

These days (as of November 2019) I work almost exclusively in python, writing scripts and packages. They are not publicly available, so I cannot link to them. But here are some tools I have been working with:

* Lots of S3 interactions, using a package I developed to wrap [`boto3`](https://github.com/boto/boto3).
* Pretty much every script and every package I write uses either [`pandas`](https://pandas.pydata.org) or  [`geopandas`](https://geopandas.readthedocs.io/en/latest/), i.e. `pandas` + the geospatial stack of [`shapely`](https://shapely.readthedocs.io/en/latest/), [`fiona`](https://fiona.readthedocs.io/en/latest/), and [`gdal`](https://gdal.org).
* I still use and love [`requests`](https://3.python-requests.org). I recently found an opportunity to create a [Custom Auth](https://3.python-requests.org/user/advanced/#custom-authentication) class, and it works like an absolute dream.

## Container Service
[Source repo](https://github.com/nrgxnat/container-service)

The container service is a plugin for the [XNAT](http://xnat.org) imaging web application, written in Java 7. It integrates a docker application into XNAT, providing new XNAT APIs to launch containers on docker.

This was a multi-year project, during which time I wrote almost the entire back end myself.

## Data Science

### Kaggle

I have completed my first "kernel" on [Kaggle](http://kaggle.com). It is an exploration of the classic beginner example Titanic data set, [My Take on the Beginner Titanic Kernel](https://www.kaggle.com/flavin/my-take-on-the-beginner-titanic-kernel).

### Applied Data Science with Python Specialization

[Coursera site](https://www.coursera.org/specializations/data-science-python)

This is a set of courses on Coursera that I will complete. I do not intend to gain the certification, but I will be working through all the assignments and posting them to a repo on github ([johnflavin/coursera-data-science-python](https://github.com/johnflavin/coursera-data-science-python)).

- [x] Intro to Data Science in Python ([Assignments](https://github.com/johnflavin/coursera-data-science-python/tree/master/01-intro-to-data-science-in-python))
- [x] Applied Plotting, Charting & Data Representation in Python ([Assignments](https://github.com/johnflavin/coursera-data-science-python/tree/master/02-applied-plotting-charting-and-data-representation-in-python))
- [x] Applied Machine Learning in Python ([Assignments](https://github.com/johnflavin/coursera-data-science-python/tree/master/03-applied-machine-learning-in-python))
- [X] Applied Text Mining in Python ([Assignments](https://github.com/johnflavin/coursera-data-science-python/tree/master/04-applied-text-mining-in-python))

## Game projects

### _morseCodeMaster
[Page on GGJ Site](https://globalgamejam.org/2018/games/morsecodemaster)
[YouTube video](https://youtu.be/tJpFLr3zVv0)
[Source repo](https://github.com/pizza-quiche/ggj2018)

This was created for the 2018 Global Game Jam, which took place January 26–28 2018. The theme that year was "transmission". My team came up with the idea that you, the player, were not directly controlling the character on screen, but were sending him transmissions in Morse code instructing him how to move. To move in any of the four directions (up, down, left, or right) you had to send a Morse code signal for the first letter of the intended direction. You sent these "signals" by pressing the space bar either a short time (a dot) or a long time (a dash). For example, to move the character up you would send the Morse code for the letter U: dot dot dash.

This game was created using Game Maker 2. The jam was the first time I had used this engine, so it was a fun opportunity to learn the engine and the Game Maker Language. (Though learning GML is really more about learning the API they provide than the language syntax itself, but that's a side point.)

My team was made up of two programmers and one artist. I programmed the Morse code input parsing, most of the movement, AI behavior (such as it was), collisions, death, menus, the secret Easter egg, and probably other things I am forgetting. My counterpart did the procedural level generation and manually created another level, sounds, and also probably other stuff.

## Unreal Engine 4 Tutorial

I have completed a game tutorial course on Udemy, [Unreal Engine 4: How to Develop Your First Two Games](https://www.udemy.com/unreale4/learn/v4/overview). Check out my [certificate of completion](https://www.udemy.com/certificate/UC-K6PQGTPM/)!
