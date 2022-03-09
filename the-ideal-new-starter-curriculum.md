# The Ideal New Starter Curriculum

## Things to learn in your first month of a new tech job

*Let's imagine a company called AwesomeCo, which has a product called Productify. This article is my conception of the sort of document I would like to receive on my first day as a new software developer at AwesomeCo (joining the Productify product team). Managers and mentors, please consider this as a starting point in your preparation for receiving new joiners to your team in future.*

## The Ideal Productify New Starter Curriculum

*Originally written for my company's intranet, July 2020.*

### Productify New Starter: Training Checklist and Curriculum

This document aims to provide you with a simple way for you to track your training over your two months at AwesomeCo. You'll get a briefing from your mentor/manager on how to best use it but here are some key points to remember:


- It is **always** OK to ask questions & generally to not know something! 
- If particular styles of learning (e.g. reading, videos, tutorials) are more effective for you, then discuss with your mentor and swap the tasks out for ones that are more suitable.
- Completing this checklist doesn't imply that your training period is over, training is something that we will always commit significant amounts of time to at AwesomeCo. This checklist is just a good place to start from. 
- This list is not in priority order. You should discuss with your mentor which things are most important to do first.

## Timeline

Below gives a rough guide for items to be completed over your first few months.

### First Day

- Welcome lunch, introduction to wider office.
- Tour of office including shower/toilets, kitchen facilities, secretarial staff, nearby amenities, office alarm system.
- Set up your work laptop, including code editor and Dev VM if needed.
- Introduction to mentor and management line.
- Social session with other new/recent starters 

### First Week

- New starter timetable for first three days of work: this should outline a number of organized workshops and meetings which should cover some of the items in this list. 
- Check off everything on the Productify "On-boarding: First week" checklist, a paper copy of this should have been given to you by your mentor.
- Make sure you've skimmed through the Productify learning, training and development resources in your first week. As you come across useful training resources - please update the intranet articles/post on internal communication channels/keep your own list to share. 
- Preparation to join scrum processes: Design a Jira/Github dashboard that displays the current Sprint [with a link to your first Jira task/New starter story] - ready to be used in stand-up on day 3. 
- HR tasks - compliance training, contact details, whereabouts, next-of-kin info.
- Who’s who in the company (AwesomeCo product areas, heads of engineering, CEO etc)
- Get set up with new laptop
- Meet and greet with team members, ice-breaker activity.
- Learn about employee groups that might be of interest, e.g. parents and carers' group, Womxn at AwesomeCo group (be offered a secondary mentor from one of these groups, if desired) 
- Learn about Productify from the customer facing manuals.
- Agree with your mentor the best order to approach the Application Development and Technology/Theory tasks below.

### Second Week

- C-programming tasks  [links to team project board] 
- Python programming tasks [links to team project board]

![Photos: CC BY 3.0 US Mapbox Uncharted ERG](https://cdn.hashnode.com/res/hashnode/image/upload/v1619963964866/76JH3q3ts.jpeg)

## Application Development

This section aims to takes you through the basics of having a problem, producing some code to solve it, putting that code somewhere where it can run and then making sure that it's running properly.

### General Programming

 - Algorithms & Data Structures
    - Complete https://www.coursera.org/learn/algorithms-part1 unless you've covered this topic at university/somewhere else (you may want to start with the basic Python/C course first)
- Python
        - Using a Pluralsight free trial to go through https://www.pluralsight.com/courses/python-getting-started
        - Complete Python Programming Exercise: WORDS and have your code reviewed by your mentor (and then by your tech lead)
        - Consider using the 'Top Trumps' exercise. 
- C
        - Ask your mentor for which chapters of the K+R book you should read. 
        - Some explanatory videos on more complicated topics  can be found here.
        - Write a "Top Trumps" style game in C.

### Productify

 - What is Productify?
    - What is Productify?
    - Find more resources here: [links]
- Productify in networks
        - Read the Productify Network Integration guide: [link]
- Learn about Productify’s CLI
        - Read the introduction sections of the CLI reference: [link]  
        - Book a Productify on [internal booking system], log onto it and play with the CLI, using the reference guide.
        - Can you configure a new user?
        - Can you configure x?
- Learn how to get diagnostics from Productify
        - Navigate the craft menu
        - Learn some cheat commands: [link]
- Learn how to upgrade Productify and apply an efix

### CI/CD

#### Git basics
- Read through https://chris.beams.io/posts/git-commit/#seven-rules explaining how to write good git commit messages
- Complete https://www.katacoda.com/courses/git

### Docker and Gitlab CI/CD training – to be researched by you.

- [example resource]
- First two sessions of https://go.digitalocean.com/containers-and-microservices.html

### Testing

#### Why is testing important?
- Read The Testing Manifesto [link]
#### Test strategy
- Work through Test Strategy [link]
- Write a test plan for a work item (link examples here) and get it reviewed by an experienced engineer.
#### Productify test frameworks
- Framework 1 (unit tests)
    - Have a look in your codebase for examples of these
    - Learn how to run a test and read the results
- Framework 2 (integration tests)
    - Learn about framework 2: [link to documentation]
    - Find a test suite and trace the keywords back to the underlying infrastructure code written in Python.
    - Run a single test, a suite of tests and tests with certain tags.
    - Look at the test log
    - Find internal trace for the tests you ran.
- Live testing
    - Learn how to run end-to-end test scripts

### Technology/Theory

This section aims to give you a basic grounding in computers, networks & various technologies that will come up in conversation time and time again as an engineer.

#### Linux (CentOS 7)
- Get familiar with basic Linux commands by doing [Linux Survival](https://linuxsurvival.com/linux-tutorial-introduction/) 
- This article (link) lists some helpful Unix and AwesomeCo specific commands.
- For complete UNIX novices, this [tutorial](http://www.freeos.com/guides/lsst/) takes you through the basics of UNIX shell syntax.

#### Networking and Protocols
- Get some coffee and read (What Happens when you type a URL into a browser)[https://medium.com/@maneesha.wijesinghe1/what-happens-when-you-type-an-url-in-the-browser-and-press-enter-bb0aa2449c1a], take notes on anything you don't understand to discuss with your mentor... if you want to go really deep check out [What Happens When](https://github.com/alex/what-happens-when).
- Read https://www.geeksforgeeks.org/domain-name-server-dns-in-application-layer/ for an introduction to DNS.
- Read  https://developer.mozilla.org/en-US/docs/Web/HTTP/Overview followed by https://www.geeksforgeeks.org/difference-between-http-and-https/ for an understanding of HTTP and HTTPS and how they differ.
- TCP/UDP - https://networklessons.com/cisco/ccna-routing-switching-icnd1-100-105/introduction-to-tcp-and-udp
- IP - https://computer.howstuffworks.com/internet/basics/what-is-an-ip-address.htm
- SIP
    - [internal powerpoint link] 
    - http://arstechnica.com/business/2010/01/voip-in-depth-an-introduction-to-the-sip-protocol-part-1/1/
    - The source! https://www.ietf.org/rfc/rfc3261.txt sections 1-5
    - Draw the SIP flow for a basic call and talk it through with your mentor.
- Read https://www.geeksforgeeks.org/rest-api-introduction/ for an introduction to REST.

![Photos: CC BY 3.0 US Mapbox Uncharted ERG](https://cdn.hashnode.com/res/hashnode/image/upload/v1619964131035/HjFpnYTfO.jpeg)

## Infrastructure and Tools

This section covers a more detailed look at how we in Productify do our day-to-day work. By the end of it you should be familiar with the concepts and have some confidence in how the platform hangs together and how to make changes.

### Writing code

#### Bash
- Complete course/read documentation
#### Sublime / VSCode / Code Editor
- Learn editor shortcuts [LINK]
- Be able to navigate the Productify codebase

### Productify work flow

- Read about the Productify Development process [link]
- Git branching strategies
    - Understand Git first!
#### Code review
- Understand why it is important to get your code reviewed
- Write some code and get it reviewed using Reviewboard, or GitLab (whatever platform you use here)

### Debugging

- General debugging theory
- Practise debugging some simple Python, after learning some Python basics.

### Agile

#### Scrum
- Read the Agile Manifesto
- Find out what scrum ceremonies your team implements, and how their sprints work.
- Go to another team's scrum ceremonies and make notes on how they are different.

### Infrastructure 

#### Jira/Trello/GitHub
#### The Productify release schedule
#### Using Slack/Discord
- Ask your mentor which channels you should join.
#### Using Zoom/Video Conferencing software
- Book a meeting with your mentor using your email calendar and link it to a video meeting. 
- Look up someone you’ve never spoken to before and video call them.
#### SFR/Bug system
- Find out if there are any bugs assigned to your team for the upcoming release
- Read about the bug raising process: [link]
#### PRD/product requirements system
#### Kit booking process
#### Intranet/Wiki
- How to create an article
- Where to find useful articles
#### The holiday system, Whereabouts system, Company directory
- book your first day's holiday

![Photos: CC BY 3.0 US Mapbox Uncharted ERG](https://cdn.hashnode.com/res/hashnode/image/upload/v1619964006118/56-kj2OAy.jpeg)
 
## AwesomeCo in general

- Resource about other AwesomeCo products: [link]

## Extra resources:
- Link
- Link


*Photos: CC BY 3.0 US Mapbox Uncharted ERG*
