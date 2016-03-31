# admissions
how you decide which hackers to admit to your event

## pipeline usage

admissions at its core can be divided into 4 main steps:

#### criteria formulation

how do you decide which people you want to have at your hackathon? do you care more about having experienced hackers who will build really cool things, or new and passionate hackers eager to learn? do you want a cohesive community that mentors each other, or people to focus on getting stuff done? do you want really cool technical hacks, or socially impactful ones? obviously these are not dichotomies, but you should decide what basis you are going to use to decide who to invite to your hackathon.

or do you want to use a lottery? let everybody in? if you don't want criteria, skip admissions completely.

#### application formulation + deployment

i recommend the use of [typeform](http://typeform.com) to do your apps. it's a beautiful form that exports easily to .csv, which makes reading + analysis a lot easier.

a template application is viewable [here](https://hackathons.typeform.com/to/hv3EiH) with some pointers. some important things to note:
1. keep it relatively short; hackers get bitter if you go over 3 or 4 longer questions, and keeping it to 1 or 2 is good
2. the current excel sheets only support around 20 questions (including name, etc.) - you shouldn't need more than that
3. keeping it at one link per field, vs. a "links" question, makes it a lot easier to read later with this interface
4. put demographic questions at the end to fight [stereotype threat](https://en.wikipedia.org/wiki/Stereotype_threat)

#### application reading

#### processing and acceptance

## a note on software
this admissions stack is done basically entirely in microsoft excel. a full web app was an option, but too time consuming; slackbots and such are options but have significant deployment costs on your end. excel allows three sheets to take care of all calculation functionality, including:
1. normalization for reader bias - some readers have higher or lower averages, or higher or lower variance
2. demographic separation - you can admit hackers with customized gender or racial breakdowns, and view your breakdowns for each method you employ

## a note on diversity
all of these tools are optimized to allow you to admit hackers with any criteria you choose (up to 5), and in any gender or racial breakdown you choose (or with no specifications). this is because of the personal bias of the creator - i believe that hackathons are fundamentally a learning experience and fundamentally about hackers and the community. when we create learning experiences, we also create opportunities to partially counteract systemic ways in which certain groups are denied access to other learning experiences, and for that reason i strongly endorse considering gender and racial breakdowns in your admissions process. when we build community, we create a group of people that is hopefully more than the sum of its individuals, something that is enhanced by a diversity of perspectives, that often come from a diversity of backgrounds and also from an atmosphere of inclusion, and for that reason i strongly endorse considering gender and racial breakdowns in your admissions process.