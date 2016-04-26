# finances
how you keep your hackathon above the red line

## budgeting

Budgeting a hackathon is hard. There's a lot of expenses; so many, in fact, it's pretty hard to predict them all at the beginning. **[Airtable](http://airtable.com)** is probably the best software to manage this - there are a few reasons that I feel this way:

1. transparency: Airtable is a collaborative platform, meaning that your entire team will be able to view (and edit, if you wish) the budget

2. attaching files: Airtable lets you attach files to each row - perfect for attaching receipts. When your team members buy anything for your hackathon, have them upload the receipt to Airtable so it's easy to process reimbursing them.

3. slack integration: Airtable can be integrated with slack such that any changes to a table are sent to a channel; this allows you to keep a log of edits to the budget.

4. categories and filters: It's easy to filter an Airtable by the category of spending or by status, making it easy to see what hasn't been bought for which parts of the event.

A template is **[here](https://airtable.com/shrfuOmq6zgSKyp7R)**; note that this budget is incomplete and most of the numbers conjured out of thin air; it's just to give you a feel for how you might set it up.

## flight reimbursements

Processing flight reimbursements - if you choose to do so - is one of the great logistical pains of hackathons, in my opinion. On the one hand, you don't want your hackers to have to pay a lot of money to come hack for a weekend. On the flip side, you're pretty constrained and want hackers to take the cheapest flight possible. Typically, a good way of reconciling this is a flight cap, or a limit on how much of each hacker's flight you'll reimburse, depending on the region they're flying from.

Setting these caps requires some research, and I'd strongly suggest **setting them right** the first time. At TreeHacks, we set them too low, and ended up having to manually raise a lot of them for our hackers; probably 30+ hours were spent on Kayak, and by the end, a couple of us could tell you off the top of our heads which flight number would get you from Boston Logan to San Francisco for $360.

Once you've set your caps, processing reimbursements should be easy, and that's what **[flightCapTable.xlsx](flightCapTable.xlsx)** is for. Copy in your RSVP data (name, email, ticket price) into the yellow space on the **rsvp** sheet. In the **raw_region_data** sheet, copy the name, email, and region columns from your **raw_data** from admissions. In the **accepted** tab, copy in your accepted list's names and emails. In the **cap_table** tab, write a list of the caps you set - i.e. northeast 350, with one region-price pairing per row. The **cap_exceptions** table is for individual names and emails to caps; hopefully if you set your caps correctly you won't need this! But if you decide that "hacker x" has a compelling reason for getting a cap raise to $500, the row will hold "hacker x", "x@gmail.com", "500".

Once you've populated all this, the **rsvp** tab should automatically compute each hackers reimbursement, and the total amount flights will cost you. remember to put an x in the check_distributed? column when you give a hacker a check!

*Note: this can also be done with a form view in Airtable, with a couple weaknesses: one being that you have to manually add the cap to each record, and the other being that you have to manually verify that each person that submits a receipt was actually accepted*

## other resources

General budgeting is a problem covered pretty extensively by **[Mackenzie's open-sourced Bitcamp budget](https://medium.com/bitcampfire-stories/bitcamps-open-source-budget-14a86974b5b2#.eyfgpq327)** and **[Ishaan from HackMIT's guide](https://medium.com/hackers-and-hacking/the-hackathon-budget-d636b5b2ed6c#.pkpwj9203)**