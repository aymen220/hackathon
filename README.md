

## Anonymous Campus Rumor System
## TEAM NAME: H.ACKERMAN
## 1. Initial Understanding
The problem is to design an anonymous campus rumor system where students can share and evaluate
information without revealing identity and without any central authority deciding what is true or false.
Instead, trust in rumors must emerge organically through user participation. The system must resist
manipulation, prevent repeated voting without identity, handle bots, explain changing trust over time, and
avoid inconsistencies caused by deleting rumors
## 2. Key Assumptions
 The system does not determine objective truth, only community trust.
 All users are anonymous; no personal identifiers are collected.
 Participation is open; users may join or leave at any time.
 Users can behave dishonestly; dishonesty is not blocked but limited in impact.
 Trust must be earned gradually through behavior, not granted instantly.
 Rumors can be related or contradictory to each other.

## 3. Core Problems Identified
- Preventing multiple votes without collecting identities
- Avoiding popularity-based truth (mob consensus)
- Handling bots and fake accounts
- Explaining trust score changes over time
- Preventing deleted rumors from corrupting trust calculations
- Ensuring resistance to coordinated attacks by liars

## 4. Proposed Solution & Features
## 4.1 Anonymous Token System
Each user receives a random local token stored on their device.
 One token = one vote per rumor
 Clearing data resets participation and credibility


## 4.2 Rumor Interaction
Users can:
 Submit rumors anonymously
 Verify or dispute rumors
 Indicate confidence level when voting
Votes are never blocked, only weighted.

## 4.3 Weighted Trust Scores
 Votes contribute unequally based on user credibility
 New users start with very low influence
 Long-term consistent behavior increases influence
This prevents popular false rumors from automatically winning.

## 4.4 Bot & Manipulation Resistance
 Bots start with minimal impact
 Credibility grows slowly over time
 Coordinated attacks require exponentially more effort
Dishonest participation becomes ineffective rather than prohibited.

4.5 Time-Based Behavior
 Older votes gradually lose influence
 Rumors lose relevance naturally
## 4.6 Handling Deleted Rumors
Rumors are archived, not deleted:
 Removed from display
 No longer affect new calculations
 Past influence on user credibility remains consistent

This prevents broken trust propagation.

- Trust Score Mechanism (Overview)
Each vote contributes:
## Vote Impact = User Credibility × Confidence Weight × Time Decay
User credibility adjusts based on:
 Consistency across related rumors
 Avoidance of self-contradictions
 Long-term participation patterns
Contradictory rumors trigger credibility updates, enabling decentralized fact-checking through behavior
rather than authority.

- Resistance to Coordinated Attacks
Because credibility grows logarithmically and resets on re-entry, attackers need a large number of long-
lived, consistent identities to influence outcomes. This makes manipulation costly and impractical without
central control.
## 7. Technologies:
Chat GPT, Gemini, Anti Gravity

## 8. Conclusion:
The system does not claim to discover truth. Instead, it models trust emergence under anonymity by
prioritizing consistency, time, and behavior over popularity or authority. This approach satisfies
decentralization while remaining resistant to manipulation.
