---
layout: page
title: Projects
permalink: /projects/
---

## Current job

The current focus of my learning is in leading and planning projects. As such I have not written as much code lately as in years past.

But I do still write some code from time to time. I'm basically writing exclusively python. My projects are not publicly available, so I cannot link to them. But some of the things I have written recently:

* A script to prepare, launch, and monitor jobs on an external service. For this project I learned a lot of new tools and techniques
    * Python's asynchronous `async`/`await` APIs and frameworks (see [Coroutines and Tasks](https://docs.python.org/3/library/asyncio-task.html)).
        * Plus a whole stack of asynchronous packages like [`aiohttp`](https://docs.aiohttp.org/en/stable/) for HTTP, [`aiobotocore`](https://aiobotocore.readthedocs.io/en/latest/) for S3, [`aioredis`](https://aioredis.readthedocs.io/en/latest/) for redis, and so on.
        * I really liked [`trio`](https://trio.readthedocs.io/en/stable/) as the concurrency backend / event loop, because I appreciated the concept of the "nursery" and [the author's take on structured concurrency](https://vorpus.org/blog/notes-on-structured-concurrency-or-go-statement-considered-harmful/). But I wasn't able to use it because I wasn't familiar enough with the ecosystem of libraries and packages, and everything I was seeing was not compatible with `trio`. I ended up using [`anyio`](https://anyio.readthedocs.io/en/stable/index.html) because it implements structured concurrency like `trio` on top of `asyncio` from the python standard library.
    * I used `redis` for object persistence.
* Worked with a team on a novel derived data format. My focus in the project was on interfaces between the science code—which implemented the underlying algorithm—and the engineering service—which wrapped around the algorithm. Some of those interfaces are the data formats in and out, function signatures, error contracts, and packaging and deployment.
* Going back a bit further, I developed and maintain a couple internal utility packages
     * A simplified package for S3, which wraps the AWS [`boto3`](https://github.com/boto/boto3) library. The main value is in handling the credential management for the user in the non-standard way my company does it. This one is very commonly used.
     * An HTTP client for a whole zoo of internal services. Again, the main value add is easy token and credential management with our internal auth mechanisms. But we also try to make it easy to add new services with as little boilerplate as possible.

## Open-source contributions

* I have contributed a few fixes and improvements to [`geopandas`](https://geopandas.readthedocs.io/en/latest/), which is a library I use at work. See [my commits](https://github.com/geopandas/geopandas/commits?author=johnflavin) on their repo.
* During my previous job I contributed to the now-defunct [spotify docker-client](https://github.com/spotify/docker-client) java library.

## Container Service
[Source repo](https://github.com/nrgxnat/container-service)

I worked on this project at a previous job. The container service is a plugin for the [XNAT](http://xnat.org) web app for medical imaging research. It integrates a docker API into XNAT, providing new XNAT APIs to launch containers on docker so researchers can run custom processing and analysis on their data stored in XNAT.

This was a multi-year project, during which time I wrote almost the entire back end myself. I wrote client APIs, service APIs, business and ORM model datatypes. It was written in Java 7 using the spring framework.

## Data Science

I have dabbled a bit with data science. I know enough to be dangerous, but it is certainly not my specialty.

### Kaggle

I have completed my first "kernel" on [Kaggle](http://kaggle.com). It is an exploration of the classic beginner example Titanic data set, [My Take on the Beginner Titanic Kernel](https://www.kaggle.com/flavin/my-take-on-the-beginner-titanic-kernel).

### Applied Data Science with Python Specialization

[Coursera site](https://www.coursera.org/specializations/data-science-python)

I completed this set of courses on Coursera. I did not gain the certification, but I worked through all the assignments and posted them to a repo on github ([johnflavin/coursera-data-science-python](https://github.com/johnflavin/coursera-data-science-python)).

- [x] Intro to Data Science in Python ([Assignments](https://github.com/johnflavin/coursera-data-science-python/tree/master/01-intro-to-data-science-in-python))
- [x] Applied Plotting, Charting & Data Representation in Python ([Assignments](https://github.com/johnflavin/coursera-data-science-python/tree/master/02-applied-plotting-charting-and-data-representation-in-python))
- [x] Applied Machine Learning in Python ([Assignments](https://github.com/johnflavin/coursera-data-science-python/tree/master/03-applied-machine-learning-in-python))
- [X] Applied Text Mining in Python ([Assignments](https://github.com/johnflavin/coursera-data-science-python/tree/master/04-applied-text-mining-in-python))

## Games

I completed a few rudimentary video games.

### _morseCodeMaster
[Page on Global Game Jam 2018 Site](https://globalgamejam.org/2018/games/morsecodemaster)  
[YouTube video](https://youtu.be/tJpFLr3zVv0)  
[Source repo](https://github.com/pizza-quiche/ggj2018)  

This was created for the 2018 Global Game Jam, which took place January 26–28 2018. The theme that year was "transmission". My team came up with the idea that you, the player, were not directly controlling the character on screen, but were sending transmissions in Morse code instructing the character how to move. To move in any of the four directions (up, down, left, or right) you had to send a Morse code signal for the first letter of the intended direction. You sent these "signals" by pressing the space bar either a short time (a dot) or a long time (a dash). For example, to move the character up you would send the Morse code for the letter U: `dot dot dash`.

This game was created using Game Maker 2. The jam was the first time I had used this engine, so it was a fun opportunity to learn the engine and the Game Maker Language and API.

My team was made up of two programmers and one artist. I programmed the Morse code input parsing, most of the movement, enemy AI behavior (such as it was), collisions, death, menus, the secret Easter egg, and probably other things I am forgetting. My counterpart did the procedural level generation and manually created another level, sounds, and also probably other stuff.

## Unreal Engine 4 Tutorial

I have completed a game tutorial course on Udemy, [Unreal Engine 4: How to Develop Your First Two Games](https://www.udemy.com/unreale4/learn/v4/overview). Check out my [certificate of completion](https://www.udemy.com/certificate/UC-K6PQGTPM/)!
