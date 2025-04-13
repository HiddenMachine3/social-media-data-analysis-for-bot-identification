# tldr;
## data cleaning :
- removed 'null_column'
- removed 100 duplicates
- corrected Follower following ratio column
## Assumptions
- influencers are accounts with lots of followers (> 6k)
- bots are accounts that raise any of the following flags:
    - too many avg likes(>70), posts(>50), comments per day(>50)
    - too much following to follower ratio (<0.2 if following count > 2000)
    - too less time between posts (<2)

# Findings : 
(look at the captions in the tableau file)
---
sentiment
- positive accounts follow more people than number of people following them. 
- negative accounts have more number of followers on average compared to neutral and positive accounts
- neutral accounts have lesser number of followers compared to negative and positive accounts
- negative accounts have more followers compared to following
---
type
- there is a higher proportion of neutral accounts among bots compared to influencer and normal types
    - this could suggest that real accounts display more emotion
- there is a lesser proportion of neutral accounts among influencers compared to normal accounts
    - this could suggest that influencers show more emotion online
- there is more proportion of negative accounts among influencers, compared to other account types.
- count of negative accounts among influencers is more compared to neutral and positive
-----


key suggestions : 
1. neutral accounts don't garner as many followers compared to emotional accounts. So having more emotional outreach might be able to garner more followers.

2. being negative is correlated with having more followers

3. Remove bots to increase authenticity

4. Focus moderation efforts more towards likely bot and negative accounts.