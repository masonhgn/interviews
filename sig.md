# SIG Interview Process (from start to finish)

Position: Software Engineer - Automated Testing
https://careers.sig.com/job/9473/Software-Development-Automated-Testing


This interview process consisted of the following rounds:
1. Take-home OA test with 2 leetcode medium questions on CodeSignal
2. Phone screen with recruiter
3. Virtual technical round via CodeSignal and Zoom with 2 engineers
4. Onsite final round at headquarters in Bala Cynwood, PA

Below I will explain each round in depth.

# TAKE HOME TEST (CodeSignal)

This consisted of 2 leetcode medium questions. The first was a hashmap / string problem, and the second was a very straightforward 2d array problem that involved manipulating a 2d array both row-wise and column-wise.


# RECRUITER PHONE SCREEN

This was a 30 minute phone call where she asked about the following:

- various questions about my background including specific stacks I used in previous roles.
- what programming languages I'm most comfortable with and why.
- some projects that I was involved with in previous roles, specific scenarios and problems I faced.
- my preference for on-site vs. remote work.
- location preferences.

This phone screen was not technical at all, and just allowed them to get to know me better.

# VIRTUAL TECHNICAL ROUND

I joined a zoom link and codesignal link, and was immediately presented with a leetcode easy level problem where I was supposed to implement a function to parse, store and lookup movies. 

The engineers offered me up to 30 minutes just to read, understand and work on the problem, and they even turned their webcams off. After asking some clarifying questions I finished the implementation in around 10 minutes, at which point they asked me to walk them through my solution. 

At this point, they started asking follow-up questions, requiring me to optimize certain things as I was trained to start with a non-optimized solution. The brunt of the interview consisted of them asking things like:

- What if we need this lookup function to be extremely fast? How might we optimize our data storage to help that?

- What was the time complexity of the old lookup function and what is the time complexity of the new one?

- What if users wanted to pass in their own criterias to load and store movies? What would be the best approach for this? (the answer he was looking for was functors).

This whole interview lasted around 1.5 hours.


# ON SITE FINAL ROUND

I entered the building at 9am using my government ID, and was met by my recruiter. After waiting around 10 minutes I was offered breakfast which I politely declined. My recruiter took me for a tour of the office which included the trading floors, all dining rooms / cafeterias, the onsite 2 story gym, fitness class rooms, barber shop, on site wellness center, and full basketball court. 

I then was taken to an interview room which contained a table with 3 chairs, some mints and water bottles, and a desk with a computer along with a projector that mirrored the computer screen.

My recruiter told me that on the computer, a coding problem would pop up at 9:45am, at which point I could read and digest it. At 10:00am, two engineers would enter, at which point I would continue reading the problem and start implementing a solution. They gave me until about 10:30 to implement a solution.


## Live Coding
The live coding portion was on CodeSignal in front of Dale and Prathun. The problem was:

- Given a set of companies which have long names and tickers, implement functions to parse through news headlines and output the tickers of the companies whose long names are mentioned.

For example:

companies = {
    "apple": "AAPL",
    "sun company": "SUNCO",
    "physics": "PHY",
    "physics corp" : "PCORP"
}

headlines = {
    "apple was trending down today at -5%, more to follow later.",
    "the physics corp has named a new ceo David Reilly today",
    "applejuice company is a new startup in silicon valley..."
}

solution: [
    ["AAPL"],
    ["PHY", "PCORP"],
    []
]

This problem looked very easy to me at first but I realized that the edge case of a company name including another company name makes it much more difficult for an O(n) or better headline parse.

### My Approach
- **Non-optimized solution:**
I tokenized each headline, created hash maps for easy lookups of long company names, and did an n² traversal to check for every possible contiguous array of tokens. I received confirmation from the interviewers that this solution was correct, but not optimal.

- **Optimized solution (incomplete):**
I initially approached this optimization incorrectly, but a solution was a trie based approach. When the interviewer explained the trie-based approach, I followed along and stepped through a specific test case, explaining my thought process and what I understood versus what I did not. I communicated my reasoning openly. Dale was transparent that they do not expect candidates to automatically know the trie solution, and emphasized that they wanted to see my thought process and communication.


## System Design
The system design portion was in front of S and P. The prompt was to design a grocery store.

### My Approach
- I began by designing a POS (point-of-sale) system with functionality to:
- Scan items one by one,
- Create and store transactions,
- Return receipts of transactions,
- Handle item returns,
- Handle discounts and coupons of varying structures.
- I started simple with a class structure and built from there.
- At times, I corrected myself and revised my data structures or functions as the interviewers added new complexity.
- I was nervous during this portion, which slightly showed.
- I fully implemented a working solution by the end.



## Manager and Behavioral Interviews

### T (Test Automation Manager)
- Tom asked me general background questions that were not very technical.
- The conversation went well overall.
- He is the manager of the test automation team, which is the team they were considering placing me on.

### S (Support Team)
- S focused heavily on my blog, particularly my post on gold/FX spot-futures arbitrage, since he had worked a lot with futures data.
- He asked about how I collected and structured my data.
- He asked me to explain my understanding of the forward carry theoretical futures pricing formula.
- He asked technical questions about memory management and lazy loading, and also asked about the Java garbage collector.
- My answers on those technical questions were correct at a high level, though not perfect.
- I would say that roughly 90% of the discussion went very well, and I was able to explain my technical understanding in depth.

### D (Data Preprocessing Team)
- D asked questions about my previous internship at a crypto trading fund.
- He asked me to explain the structure of decentralized exchanges.
- He asked me to explain the differences and tradeoffs between various decentralized swap protocols.
- I was able to answer these questions correctly and confidently.
- I was transparent that I had limited knowledge before that internship, but I demonstrated what I learned and how I thought about the material.

### K (T’s Manager)
- K asked many questions about my preferences and past projects.
- He asked where I prefer to work, and what management style I like.
- He asked me to describe a project I was proud of, and a project I was not proud of, including the reasons why.
- I believe this conversation went very well.


## Recruiter Wrap-Up (V)
- V asked me how everything went and which teams I liked talking to the most.
- She asked whether I had any competing offers or deadlines.
- She asked about my salary expectations. I told her that I did not know what to expect regarding salary.
- She asked, if I did have multiple offers, what my biggest deciding factors would be.
- She asked if I would want to live in Philadelphia. I told her that I would love to live in Philadelphia.
- I also said that I liked the test automation and support teams, but that I genuinely enjoyed speaking with all of the teams.


## Closing (J)
- J gave me a gift bag containing a sweater and a deck of cards.
- She offered me more food.
- She then walked me out.



# Extra Details

### Times to hear back between rounds:
1. OA -> phone screen: 1 week
2. phone screen -> technical: 10 minutes
3. technical -> onsite: 3 days
4. onsite -> decision: 4 business days


### Miscellaneous
- For the onsite, they purchased my flight to and from my home city, put me in a hotel in philadelphia from the day before my interview to the day after my interview.
- During the onsite I was given an uber eats voucher of 50 dollars and an uber voucher with 7 free rides.

