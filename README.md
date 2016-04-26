# hackathonpack
organizing a hackathon: a hackpack

## preface
A hackpack is a package of starter code that serves as, **[per treehacks](https://medium.com/@hackwithtrees/treehacks-the-redux-7f4e50feb8ba#.vkw9kbdkj)**, a tool for hackers to "help you skip the drudgery and get straight to your dreams." This is an attempt to do similar for organizers. When it comes to hackathons, too many events suffer because a lot of time is spent on the menial work - the mechanics of admissions, money, or logistics, for instance - and organizers don't have time to plan the "non-essentials," like extra experiences or great ceremonies, to take their events to the next level.

This is a guide, and more importantly, "software" stack + suggested softwares, to help you do the easy stuff more efficiently. It is by no means meant to be a replacement for the **[mlh organizers guide](http://guide.mlh.io/)** - you should think of that as a more linear narrative to help plan a hackathon, while this is a set of tools that you pick and choose from to deploy as you need them.

(Almost) all of this has been "battle-tested" by organizing teams, and we'd love to see organizing teams who have processes for their hackathons contribute as well. Hundreds of hackathons are run across the country - it seems that every hackathon could gain a lot if we all shared our methods, best practices, and tools.

## how to use
Each folder (the complete list of folders is available in the index section below) has a README, which explains the various tools included. Some tools (admissions in particular) require a pretty stringent process to remain clean and easy to use - if this is the case, it'll be detailed in the README.

This should go without saying, but use whichever modules you have a need for/you feel will work well for you. each folder is independent and can be used as such.

My suggestion would be to fork this repo right away for your team.

Sometimes the README will link to software that has been open-sourced by a hackathon vs. something that was contributed directly to this hackpack - everything that is linked to will be open-source, though.

## section index

### admissions

1. hackathonAppReading - a tool process copy/pasted typeform data and use searches to read apps

2. hackathonAppScoring - a tool to record hackerID-score tuples and have them automatically normalized for reader bias

3. hackathonAppProcessing - a tool to aggregate copy/pasted normalized scores from 2. and use some configurations to pick admits

4. README - explains the above 3 in greater depth, and adds:

  1. Hackathon Application Template - a typeform with some examples and pointers for setting up a Typeform application

### finances

1. flightCapTable.xlsx - a tool to integrate ticket price and flight caps based on region, and verify acceptance, to compute reimbursement for each hacker

2. README - airtable budget template and explanation of flight cap table

### internal

1. README - a brief rundown of suggestions for keeping your team organized

### judging

1. judgingcriteria.pdf - a sample explanation of judging criteria to provide to the judges

2. judgingsheet.pdf - a sample judging sheet to provide to the judges

3. judging.sketch - the source file (Sketch) for the above

4. judgingrecord.xlsx - a tool to aggregate judges' scores for hacks and pick a top twenty, from which we recommend the judges/organizers manually narrow down the top x

5. README - explanation of the above tools, as well as devpost suggestions and a link to treehacks' open source SMS based judging pipeline

### registration

### partnership

## additional resources

## acknowledgments

Assembled by **[mike](http://mikeyu.me)**, who thanks **[TreeHacks](http://treehacks.com)**, **[Cal Hacks](http://calhacks.io)**, and **[The Big Hack](http://bighack.org)** for building great hackathons he got to be a part of. Thanks also to **[Camille](http://camilleconsidine.com)** for her extensive work on sponsorship research and for deploying a number of these tools for the first time at **[Bayes Hack](http://bayeshack.org)**. Also special shout to **[TreeHacks](http://treehacks.com)** for making the effort to outsource a lot of their tech tools which are linked extensively throughout.