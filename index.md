## Table of contents

* [Overview](#overview)
* [User Guide](#user-guide)
* [Community Feedback](#community-feedback)
* [Developer Guide](#developer-guide)
* [Development History](#development-history)

## Overview

COVID Kōkua is a web application that uses crowdsourcing to collect, organize and present helpful resources to combat the effects of COVID-19, including:

- Financial Aid
- Unemployment Programs/Assistance
- Links to official hotlines or contacts
- A help-ticket system to answer additional questions users may have

## User Guide

This section provides a walkthrough of the COVID Kōkua user interface and its capabilities.

### Landing Page

The landing page is presented to users when they visit the top-level URL to the site.

![](images/landing-page.png)

### Index pages (Financial Aid, Unemployment Help, COVID News)

COVID Kōkua provides three public pages that present the contents of the database organized in various ways.

### Home page

After logging in, you are taken to the home page, which presents a form where you can complete and/or update your personal profile:

![](images/home-page.png)

## Developer Guide

This section provides information of interest to Meteor developers wishing to use this code base as a basis for their own development tasks.


### Application Design

COVID Kōkua is based upon [meteor-application-template-react](https://ics-software-engineering.github.io/meteor-application-template-react/) and [meteor-example-form-react](https://ics-software-engineering.github.io/meteor-example-form-react/). Please use the videos and documentation at those sites to better acquaint yourself with the basic application design and form processing in Kōkua.


### Quality Assurance

#### ESLint

Kōkua includes a [.eslintrc](https://github.com/bowfolios/bowfolios/blob/master/app/.eslintrc) file to define the coding style adhered to in this application. You can invoke ESLint from the command line as follows:

```
meteor npm run lint
```

Here is sample output indicating that no ESLint errors were detected:

```
$ meteor npm run lint

> bowfolios@ lint /Users/philipjohnson/github/bowfolios/bowfolios/app
> eslint --quiet --ext .jsx --ext .js ./imports ./tests

$
```

ESLint should run without generating any errors.

It's significantly easier to do development with ESLint integrated directly into your IDE (such as IntelliJ).
