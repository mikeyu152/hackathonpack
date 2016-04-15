# judging
allocating prizes and all that fun stuff

## how important is judging?
hackers seem to want to move away from competition, at least if social media is to be believed. "hacking should be done for hacking's sake" is not a totally crazy or out-there belief. however, if your hackathon has prizes (which it probably does), you'll need judges. you can give up prizes and winners, but this is a philisophical discussion your team might want to think about internally.

## getting judges

generally, it seems sub-optimal to have a lot of your organizing team judge. your organizing team isn't necessarily the best equipped to judge a hackathon, and is very likely to be running around fighting fires (metaphorically!) during expo and closing ceremony. the best judges are typically people from industry, whether that mean engineers, designers, engineering managers, etc. your sponsors will probably be busy judging their sponsored prizes (and you definitely don't want to be in a position where you are judging sponsor prizes - let them do that), so you'll probably have to pull some strings through your network.

## submissions

i'd strongly recommend running submissions (even if not judging) via [devpost](http://devpost.com). it's a generally tried and true standard, it's not hard to use, and it works well for a lot of hackers because they already have accounts and portfolios on the site. it's simple, and devpost has an extensive guide to using their platform to manage a hackathon [here](http://help.devpost.com/customer/en/portal/topics/780166-managing-your-hackathon/articles).

## expo logistics

putting an expo together is probably the most logistically challenging aspect of a hackathon, at least from a venue standpoint. plan out well in advance which space is going to be used for your expo and how that space will be configured, and make sure that the space is cleared at least an hour before expo so that your team can set it up. there's really not much to be said here, other than that you're going to need a lot of manpower to set the space up, and to get as big a space as possible with ample walkways.

another important matter is assigning tables; it's nice for your judges/sponsors if you can assign tables so that teams competing for similar prizes are reasonably close together. you'll also want to make sure hardware hacks have adequate space, and if they are hard to move, you'll probably want to leave them wherever they currently are in the space - yet another table numbering constraint.

it seems like the science fair-style expo is something that really hasn't been iterated on since the first hackathons, and space for a lot of improvement - if you try something and it works well, please submit a pull request!

## judging process

some hackathons judge on devpost with a rating system - you can learn to set that up [here](http://help.devpost.com/customer/en/portal/articles/1929826-how-judging-works---for-hackathon-managers). most hackathons seem to choose not to do this though, and they usually adopt one of two main methods for judging a large number of hacks:

#### absolute scoring

each judge gets a set of criteria, and rates each hack she's assigned on some scale, whether that's 1-5, 1-10, or something else. if you go this route, a sample judging sheet is included [here](judgingsheet.pdf) - it was used at the 2016 big hack. the raw sketch file for these files is [judging.sketch](judging.sketch) if you use sketch - the one thing i would always recommend for judging sheets with this kind of scoring is to make sure judges can fold the scores behind, so they don't have to worry about hiding them from the teams while talking.

if you go this route, you can use [judgingrecord.xlsx](judgingrecord.xlsx) to record the scores as they come in via your judges sheets. as always, edit the boxes that are yellow. use the **config** tab to pick your three criteria and input the number of tables, as well as how you want each criteria to be weighted. as the judging sheets come in, each judging of a table just gets another entry in the **data** sheet - add table number and the three criteria to a new row. the **scoring** sheet automatically averages all the scores and computes a total and rank, and the **top_twenty** sheet lists the top twenty table numbers. we use top twenty because at this point you probably want to have the judges talk a bit and/or go check out the contenders to narrow it down to the winners who will demo or take home prizes.

#### top of batch

another technique that has been used for large(r) hackathons has been to assign each judge some batch of tables (say, 8), and pick a top one or two from that batch; this process then gets repeated until winners are picked. treehacks has an open-source API to use twilio to do this via sms [here](https://github.com/TreeHacks/Judging-API)
