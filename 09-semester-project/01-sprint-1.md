# Semester Project

## Setting up student meeting times
1. Each team will have a virtual deployment machine that I provide. It will have sufficient disk space and 12 GB of virtual RAM. 
2. We will work together to discuss the requirements you will work on, and organize your projects. 
3. Times I have set aside right now are: 
    - Noon - 8pm Wednesday, October 28
    - 11am - 5pm Thursday, October 29
    - Noon - 6pm Sunday, November 1
4. You will each have an Augur Database at your disposal, and installed for you in your VM. It will have data from a set of 92 Scientific Open Source Software Projects. There are three repositories you can use in different combinations to address the requirements for your project. 
    - https://github.com/chaoss/augur (required)
    - https://github.com/chaoss/augur-community-reports 
    - https://github.com/chaoss/augur-spdx 
5. There are related projects that you may consider incorporating into Augur as well. These include: 
    - https://deps.cloud/ -- They need a PyPi dependency collector at the moment
    - https://github.com/indeedeng/Mariner-Issue-Collector - Here, you could take a list of GitHub repositories from an Augur instance and gather information on issues recently opened. 

## Resources for Getting Started and Requirements (All groups need at least one use case, including the diagram. Some groups may be able to more easily express the details of their requirements narratively or in the spreadsheet template from module 3)
 - [Use Case Template](./_use-case-template.md)
 - [Requirements Template from Module 3](https://github.com/MUSoftwareEngineering/CS-4320/blob/master/03-requirements/readings/requirements-template.xlsx)

### Augur Software
![](./images/augur-map.png)
1. [Augur Documentation](https://oss-augur.readthedocs.io/en/dev/)
2. [Augur Community Reports Repo](https://github.com/chaoss/augur-community-reports)
3. [Slack Bot "Auggie"](http://auggie.augurlabs.io/#/login)
4. http://augur.osshealth.io:5055/api/unstable/repos
5. [Contributor Analysis from augur-community-reports](https://docs.google.com/presentation/d/1rLuEROyKlujjPd9AEQ5z1v0V1WPYagv454SBHFNpRDU/edit#slide=id.g8b77fbdb00_0_5)

### Augur Documentation
1. [Conceptual Overview of Augur Data](http://www.augurlabs.io/under-the-hood-with-augurs-data/)
2. [Augur's Full, physical data model](http://www.augurlabs.io/augurs-full-physical-data-model/)
3. [Creating an Augur Worker](http://www.augurlabs.io/learn-how-to-create-an-augur-worker/)
4. [CHAOSS Committers Metrics](https://chaoss.community/metric-committers/)
5. [CHAOSS Risk Metrics](https://chaoss.community/metrics/#user-content-focus-area---business-risk)
6. [Currently open Augur Issues](https://github.com/chaoss/augur/issues)

### Candidate Ideas
0. [Metrics Currently Under Development That You Could Create EndPoints For](https://docs.google.com/spreadsheets/d/1tAGzUiZ9jdORKCnoDQJkOU8tQsZDCZVjcWqXYOSAFmE/edit#gid=1004270137)
1. Front end fixes
2. Debugging and deploying machine learning workers (gsoc-dev branch)
3. Ecosystem Level Queries and Analysis
4. Documentation Updates, especially developer instructions
5. Containerization of augur-spdx
6. Frontend redesign or new front end using tools like Graphana 
7. Many, many more to discuss!


## Schedule and Deliverable Overview
![](./images/semester-project.png)
