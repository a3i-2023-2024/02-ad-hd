---
title: AI in the Industry Tutorials (Anomaly Detection via Density Estimation)
author: michele.lombardi2@unibo.it
---

# Anomaly Detection in Higher-Dimensional Spaces #

This is the first lecture block of the 2023/2023 edition of the "AI in the Industry" course, from [University of Bologna](https://www.unibo.it). Each lecture consists of a tutorial that tackles a simplified industrial problem and tackles it using AI techniques, from Machine Learning to Combinatorial Optimization (and later on their combination).

While the whole course looks like cookbook, the real goal is using examples to teach how industrial problem can be methodically approaches, analyzed, and tackles using a combination of techniques.

This tutorial in particular tackles anomaly detection in task in (relatively) high-dimensional spaces, via density estimation techniques and autoencoders. The focus is on showing how density estimation can be tackled with a broader range of techniques, and also to show how some methods that are not presented from a probabilistic perspective have indeed a probabilistic interpretation.

# Accessing the Lecture #

## Local Execution (Preferred) ##

Students are strongly encouraged to _run all lectures locally_. Doing this will require to:

* Install Docker, by following the [online instructions](https://docs.docker.com/get-docker/).
* Linux users should also install Docker Compose, by following the [online
instructions](https://docs.docker.com/compose/install/)
* Download or clone this repository, e.g. via the command:
```sh
git clone https://github.com/a3i-2023-2024/02-ad-hd.git
```
* Open a terminal in the main directory of the downloaded/cloned repository
* Start the container via Docker Compose:
```sh
docker compose up
```

On Linux systems, you may need to start the docker service first.

No matter which OS your are running, the first execution of this process will be fairly long, since Docker will need to download a base image for the container (think of a virtual machine disk) and then some boilerplate configuration steps will need to be performed (e.g. installing jupyter in the container). Subsequent runs will be much faster.

The process will end with a message such as this one:

```sh
To access the notebook, open this file in a browser:
    file:///home/lompa/.local/share/jupyter/runtime/nbserver-1-open.html
Or copy and paste this URL:
    http://127.0.0.1:39281/?token=0cd92163797c3b3abe67c2b0aea57939867477d6068708a2
```

Copying one of the two addresses in a file browser will provide access to the Jupyter server running in the spawned container. By default, the main lecture folders is shared with the container environment, so any modification you make in the contain will reflect in the host system, and the other way round.

Once you are done, pressing CTRL+C on the terminal will close the Docker container.

For more information about how Docker works (such as the difference between images and containers, or how to get rid of all of them once you are done with the tutorial), you can check the [Docker documentation](https://docs.docker.com/).

## Read-only Access and PDF Notes ##

You can inspect the individual notebooks in by just clicking on any `*.ipynb` file in the `notebooks` directory: github provides a notebook viewer that mostly works, though this access method may occasionally have issue when displaying plots.

The repository contains PDF notes for all the notebooks. They can be used for read-only access (with more consistent results compared to the github notebook viewer), but more importantly they can be useful to add annotations. Just keep in mind that in case of updates, cloning the repository will replace the PDF files.
