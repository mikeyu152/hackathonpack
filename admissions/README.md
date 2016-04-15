# admissions
how you decide which hackers to admit to your event

## pipeline usage

admissions at its core can be divided into 5 main steps:

#### criteria formulation

how do you decide which people you want to have at your hackathon? do you care more about having experienced hackers who will build really cool things, or new and passionate hackers eager to learn? do you want a cohesive community that mentors each other, or people to focus on getting stuff done? do you want really cool technical hacks, or socially impactful ones? obviously these are not dichotomies, but you should decide what basis you are going to use to decide who to invite to your hackathon.

or do you want to use a lottery? let everybody in? if you don't want criteria, skip admissions completely.

#### application formulation + deployment

i recommend the use of [typeform](http://typeform.com) to do your apps. it's a beautiful form that exports easily to .csv, which makes reading + analysis a lot easier.

**a template application is viewable [here](https://hackathons.typeform.com/to/hv3EiH)** with some pointers. some important things to note:

1. keep it relatively short; hackers get bitter if you go over 3 or 4 longer questions, and keeping it to 1 or 2 is good

2. the current excel sheets only support around 20 questions (including name, etc.) - you shouldn't need more than that

3. keeping it at one link per field, vs. a "links" question, makes it a lot easier to read later with this interface

4. put demographic questions at the end to fight [stereotype threat](https://en.wikipedia.org/wiki/Stereotype_threat)

#### application preprocessing

once you close your applications, you'll want to put the data in a place that your team can read the apps. download the .csv file from typeform, and copy paste all of the data (this supports up to 4000 applications) into the yellow highlighted space on the raw_data tabs of [hackathonAppReading.xlsx](hackathonAppReading.xlsx) and [hackathonAppProcessing.xlsx](hackathonAppProcessing.xlsx). hackathonAppReading is the sheet you will send to the rest of your team, as well as a range of hacker IDs for apps to read, and hackathonAppProcessing is the system used to aggregate reader ratings and pick hackers.

#### application reading

distribute a copy each of [hackathonAppReading.xlsx](hackathonAppReading.xlsx) (the version you pasted the data into) and [hackathonAppScoring.xlsx](hackathonAppScoring.xlsx) to each of your readers, along with a range of hacker IDs for applications they are responsible for (example: if i were running a hackathon and giving each hacker 2 reads, had 1000 apps, and 20 team members, i might give ranges 1-100, 51-150, 101-200, etc, to each of my team members - somebody would get 1-50 and 951-1000; the ranges don't have to be contiguous).

not every hacker has to get the same number of reads - the sheets compute each hacker's average scores.

the reading process for your readers looks roughly as follows:

1. open hackathonAppScoring, and on the **config** tab, type the reader's name and the criteria by which apps are being judged (this criteria should be the same for all readers)

2. type the hacker id of in the yellow box on the **app_reading** sheet of hackathonAppReading. read the app - links for hyperlinks are next to the field if the field is a URL (this is why only one link per question, with typeform's link field, is best).

3. in hackathonAppScoring, in the **scoring** sheet, type the hacker ID, score for each criteria, and any notes on a new row in the yellow box. try to use notes sparingly. which scoring system is used is not important, although i recommend either a 1-5 or 1-7 scale, with an attempt to squeeze towards the middle.

4. when done reading all apps, save hackathonAppScoring and send it back to whoever is running processing

#### processing and acceptance

when processing, you'll have received a bunch of scoring sheets from your readers. the first thing you need to do is aggregate this data. just copy the entire contents of the **output** tab (any numbers that come up in the teal boxes) of each hackathonAppScoring sheet, and paste into the **normed_score_inputs** tab of hackathonAppProcessing. **when pasting, right click, choose "paste special", and choose "paste as values"**.

after doing this for all the sheets, you should have all of the scores with weird decimal numbers in the yellow columns (the numbers are z-scores - we normalize each score into a z-score based on the distribution of the reader).

at this point, you have three choices:

1. accept the *n* highest scores. to do this, use the **acceptance_panel** sheet of hackathonAppProcessing, and configure the yellow box for the number of people you want to accept to your hackathon. the stats will tell you how many you actually accepted (should match the yellow box, unless you don't have enough applicants... or you're trying to accept more than 3000 hackers), and give gender and racial breakdowns of your accepted pool. their info is below the line; you're good to go!

2. accept the *n* highest scores subject to some desired gender breakdown. to do this, use the **gender_diversity_acceptance** sheet of hackathonAppProcessing, and configure the yellow boxes for the number of people you want to accept to the hackathon, and the gender breakdown you're looking to accept - this breakdown must add up to 1. the stats will tell you how many you actually accepted, and give gender and racial breakdowns of your accepted pool. their info is below the line; you're good to go!

3. accept the *n* highest scores subject to some desired racial breakdown. to do this, use the **racial_diversity_acceptance** sheet of hackathonAppProcessing, and configure the yellow boxes for the number of people you want to accept to the hackathon, and the racial breakdown you're looking to accept - this breakdown must add up to 1. the stats will tell you how many you actually accepted, and give gender and racial breakdowns of your accepted pool. their info is below the line; you're good to go!

typically it's a good idea to use 1. first, to gauge what the breakdown looks like with no restrictions, and adjust from there to try and build a diverse/worthwhile community and specify that breakdown.

## a note on software
this admissions stack is done basically entirely in microsoft excel. a full web app was an option, but too time consuming; slackbots and such are options but have significant deployment costs on your end. excel allows three sheets to take care of all calculation functionality, including:

1. normalization for reader bias - some readers have higher or lower averages, or higher or lower variance

2. demographic separation - you can admit hackers with customized gender or racial breakdowns, and view your breakdowns for each method you employ

## a note on diversity
all of these tools are optimized to allow you to admit hackers with any criteria you choose (up to 5), and in any gender or racial breakdown you choose (or with no specifications). this is because of the personal bias of the creator - i believe that hackathons are fundamentally a learning experience and fundamentally about hackers and the community. when we create learning experiences, we also create opportunities to partially counteract systemic ways in which certain groups are denied access to other learning experiences, and for that reason i strongly endorse considering gender and racial breakdowns in your admissions process. when we build community, we create a group of people that is hopefully more than the sum of its individuals, something that is enhanced by a diversity of perspectives, that often come from a diversity of backgrounds and also from an atmosphere of inclusion, and for that reason i strongly endorse considering gender and racial breakdowns in your admissions process.