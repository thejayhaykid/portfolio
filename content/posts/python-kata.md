---
title: "Babysitter Kata"
date: 2019-11-26
lastmod: 2019-11-26
draft: true
description: "Using test driven development to solve a problem."
show_in_homepage: false
show_description: false
license: ''

tags: ['Python','kata','test-driven-development','pytest']
categories: ['Python']

featured_image: ''
featured_image_preview: ''

comment: true
toc: true
autoCollapseToc: true
math: true
---

# Babysitter Kata

[Description of the Problem](https://github.com/PillarTechnology/kata-babysitter)

[Github link to source code](https://github.com/thejayhaykid/babysitter-kata)

## Description

> This kata simulates a babysitter working and getting paid for one night. The rules are pretty straight forward.

## Initial Thoughts

For this exercise I was given the option to select my own language from a list, I decided to go with Python as it is one of the languages I am most comfortable with. After spending over a year listening to both the [PythonBytes](https://pythonbytes.fm/) and [Test & Code](https://testandcode.com/) podcasts, I had heard enough from [Brian Okken](https://twitter.com/brianokken) to use [pytest](https://docs.pytest.org/en/latest/) as the "test" part of my test driven development.

Having never used pytest before, I decided to buy [Brian's book](https://pragprog.com/book/bopytest/python-testing-with-pytest) so that I could get a good foundation of how pytest specifically worked. As a side note, I would recommend pytest if you are working on a python project. So I spent a couple of hours storming through that book so that I would have some idea of what I was doing. 

After establishing that I was going to use pytest, I planned out the rest of what I was going to use for this project. To make it easier to develop on multiple machines I decided to use virtualenv. This way to use this package on another machine, all I would need to do (after using pip to install virtualenv) is install the packages in the requirements.txt file using `pip install -r requirements.txt` and then the package is ready to go.

The other package in requirements.txt file other than pytest is [Click](https://click.palletsprojects.com/en/7.x/). Click is a very powerful package that makes adding a command line interface (CLI) to your python package very easy. Using decorators and functions, defining a CLI is very easy.