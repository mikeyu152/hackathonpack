# finances
how you keep your hackathon above the red line

## budgeting

budgeting a hackathon is hard. there's a lot of expenses

## flight reimbursements

processing flight reimbursements - if you choose to do so - is one of the great logistical pains of hackathons, in my opinion. on the one hand, you don't want your hackers to have to pay a lot of money to come hack for a weekend. on the flip side, you're pretty constrained and want hackers to take the cheapest flight possible. typically, a good way of reconciling this is a flight cap, or a limit on how much of each hacker's flight you'll reimburse, depending on the region they're flying from.

setting these caps requires some research, and i'd strongly suggest **setting them right** the first time. at treehacks, we set them too low, and ended up having to manually raise a lot of them for our hackers; probably 30+ hours were spent on kayak, and by the end, a couple of us could tell you off the top of our heads which flight number would get you from boston logan to san francisco for $360.

once you've set your caps, processing reimbursements should be easy, and that's what [flightCapTable.xlsx](flightCapTable.xlsx) is for. copy in your RSVP data (name, email, ticket price) into the yellow space on the **rsvp** sheet. in the **raw_region_data** sheet, copy the name, email, and region columns from your **raw_data** from admissions. in the **accepted** tab, copy in your accepted list's names and emails. in the **cap_table** tab, write a list of the caps you set - i.e. northeast 350, with one region-price pairing per row. the **cap_exceptions** table is for individual names and emails to caps; hopefully if you set your caps correctly you won't need this! but if you decide that "hacker x" has a compelling reason for getting a cap raise to $500, the row will hold "hacker x", "x@gmail.com", "500".

once you've populated all this, the **rsvp** tab should automatically compute each hackers reimbursement, and the total amount flights will cost you. remember to put an x in the check_distributed? column when you give a hacker a check!

