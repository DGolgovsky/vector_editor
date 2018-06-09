# grasp
Homework 05 task. [OTUS C++]

[![Build Status](https://travis-ci.org/DGolgovsky/vector_editor.svg?branch=master)](https://travis-ci.org/DGolgovsky/vector_editor)
[![Code Health](https://landscape.io/github/DGolgovsky/vector_editor/master/landscape.svg?style=flat)](https://landscape.io/github/DGolgovsky/vector_editor/master)
[ ![Download](https://api.bintray.com/packages/dgolgovsky/otus-cpp/vector_editor/images/download.svg) ](https://bintray.com/dgolgovsky/otus-cpp/vector_editor/_latestVersion)

Design of the simplest graphic vector editor.Prepared class layouts reflecting the structure of the project.

Functional for prototyping the following:

- creating a new document

- importing a document from a file

- exporting a document to a file

- creating a graphic primitive

- delete a graphic primitive

The main emphasis is on the controller template and polymorphism. Functions that are GUI handlers are compiled in one file with the main function.

Doxygen and the publication of the html-versions of documentation on github-pages.

Detailed description on the [gh-pages](https://dgolgovsky.github.io/vector_editor/)

**Example of Dockerfile**

```
FROM ubuntu:trusty
#### Bintray (by JFrog) 
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 379CE192D401AB61
#### Dmitry Golgovsky (Packages sign) 
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys D5CEB8D4D5185900
#### toolchain repo key
RUN apt-key adv --keyserver keyserver.ubuntu.com --recv-keys 1E9377A2BA9EF27F
RUN echo "deb http://dl.bintray.com/dgolgovsky/otus-cpp trusty main" | sudo tee -a /etc/apt/sources.list
RUN echo "deb http://ppa.launchpad.net/ubuntu-toolchain-r/test/ubuntu trusty main" | sudo tee -a /etc/apt/sources.list
RUN apt update
RUN apt install -y libstdc++6 vector_editor
```

# OTUS-Cpp
OTUS C++ online [course](https://otus.ru/lessons/razrabotchik-c++/) studying repository.

**About the course**

Being one of the most popular programming languages, C++ is widely used for software development. Scope of usage includes the creation of operating systems, a variety of applications, device drivers, applications for embedded systems, high-performance servers, and entertainment applications (games).
In the course "C++ Developer" will be considered as introductory concepts, such as automation tools, STL, innovations of `11` and `14` standards; and more complex: asynchronous programming, design patterns, distributed high-availability services architectures.
