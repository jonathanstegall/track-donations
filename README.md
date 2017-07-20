# Track Donations
Web app used to track donations based on how much you tell it you make, how much you tell it you've already given, and what percentage you tell it you'd like to give.

## Basic data concept

1. Table for income - supply it with date, amount, recipient name (like for couples), notes
2. Table for donation payments - supply it with date, amount, where it's going, maybe notes
3. Table for recurring donations - supply it with a way to link to individual donation payments, plus amount, recurrence, where it's going, notes.
4. Options - what percentage you'd like to give, maybe storing the names of commonly occurring things, time periods to track (ie track your monthly donations)

## Basic form concepts

1. Add/edit/delete an income transaction
2. Add/edit/delete an individual donation (ie give to a disaster relief that doesn't repeat automatically)
3. Confirm a recurring thing actually happened (ie you actually did give money to your church this month)
4. Update percentage option, any other options

## Basic display concept

1. Forms above
2. How much you've already given this time period in total and percentage of tracked income
3. How much you have left to give this time period if you want to meet your goal (can be negative if you go over)

## Data storage

I'm not convinced any of this data needs to be stored on a server. Maybe if it's somehow anonymized? But I think storing it locally on the user's device (with HTML5 or whatever) is perhaps better than dealing with the privacy implications of people storing what percentage people want to give away, what amounts they receive, and what amounts they give away.

While storing the data locally does make it volatile in its on way, to device loss or data expiration or any number of things, it seems worthwhile. Maybe remind users to export it from time to time if they want to save it somewhere.
