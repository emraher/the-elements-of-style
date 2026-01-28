# The Elements of Style (1918) - Condensed

*Public domain text by William Strunk Jr.*

## Core Principle

Write clearly. Cut ruthlessly. Every word must earn its place.

## II. Elementary Rules of Usage (Grammar/Punctuation)

**Rule 1.** Form possessive singular by adding 's: Charles's friend, Burns's poems.

**Rule 2.** In a series of three or more, use comma after each term except the last: red, white, and blue.

**Rule 3.** Enclose parenthetic expressions between commas. Never one comma without the other.

**Rule 4.** Comma before conjunction introducing co-ordinate clause: "The situation is perilous, but there is still one chance."

**Rule 5.** Do not join independent clauses by comma. Use semicolon or period: "It is nearly half past five; we cannot reach town before dark."

**Rule 6.** Do not break sentences in two. Do not use periods for commas.

**Rule 7.** Participial phrase at beginning must refer to grammatical subject.
- Wrong: "Walking slowly down the road, a house came into view."
- Right: "Walking slowly down the road, he saw a house."

## III. Elementary Principles of Composition

**Rule 8.** One paragraph per topic. Each paragraph signals a new step in development.

**Rule 9.** Begin paragraph with topic sentence. End in conformity with beginning. Avoid ending with digression or unimportant detail.

**Rule 10. Use active voice.**

Active voice is more direct and vigorous:
- Weak: "My first visit to Boston will always be remembered by me."
- Strong: "I shall always remember my first visit to Boston."

Replace perfunctory expressions:
- Not: "There were dead leaves on the ground."
- But: "Dead leaves covered the ground."

**Rule 11. Put statements in positive form.**

Make definite assertions. Use *not* for denial or antithesis, never for evasion:
- Not: "He was not very often on time."
- But: "He usually came late."
- Not: "did not remember" → But: "forgot"
- Not: "not honest" → But: "dishonest"

**Rule 12. Use definite, specific, concrete language.**

Prefer specific to general, definite to vague, concrete to abstract:
- Not: "A period of unfavorable weather set in."
- But: "It rained every day for a week."
- Not: "He showed satisfaction as he took possession of his reward."
- But: "He grinned as he pocketed the coin."

**Rule 13. Omit needless words.**

Vigorous writing is concise. Every word must tell.

Common violations:
- "the question as to whether" → "whether"
- "there is no doubt but that" → "no doubt"
- "used for fuel purposes" → "used for fuel"
- "he is a man who" → "he"
- "in a hasty manner" → "hastily"
- "owing to the fact that" → "since"
- "in spite of the fact that" → "though"

Eliminate "the fact that" from every sentence.

**Rule 14.** Avoid succession of loose sentences. Vary sentence structure to prevent monotony.

**Rule 15. Express co-ordinate ideas in similar form.**

Parallel construction lets readers recognize likeness of content:
- Not: "Formerly, science was taught by textbook, while now the laboratory method is employed."
- But: "Formerly, science was taught by textbook; now it is taught by laboratory method."

**Rule 16. Keep related words together.**

Position shows relationship:
- Not: "He only found two mistakes."
- But: "He found only two mistakes."
- Not: "There was a look in his eye that boded mischief."
- But: "In his eye was a look that boded mischief."

**Rule 17.** In summaries, keep to one tense. Use present for drama, present or past for narrative.

**Rule 18. Place emphatic words at end.**

The most prominent position is the end:
- Weak: "Humanity has hardly advanced in fortitude since that time, though it has advanced in many other ways."
- Strong: "Humanity, since that time, has advanced in many other ways, but it has hardly advanced in fortitude."

## V. Words Commonly Misused (Condensed)

**Wordiness**: case, character, nature, factor, feature, interesting → Cut them
- "In many cases" → "Many" | "Acts of hostile character" → "Hostile acts"

**Wrong substitutions**:
- claim ≠ say/declare | state ≠ say | possess ≠ have/own | fix ≠ arrange
- like ≠ as (use *as* before clauses) | most ≠ almost | while ≠ and/but/although

**Grammar**:
- data/phenomena/strata = plural | different from (not than)
- less = quantity, fewer = number | effect = result, affect = influence

**Avoid**: "as to whether" (use whether), "due to" as adverb (use because of), "etc." after "such as", "the fact that" (always rewrite), "one of the most" (tired), "so/very" as intensifiers, "respective/respectively" (usually omit)

**Logic**: but unnecessary after doubt/help | however as "nevertheless" can't start sentence | literally ≠ figuratively | shall (1st person future), will (determination)

## Application to Technical Writing

Apply Rules 10-13 and 16 to all technical prose:

### Git Commit Messages (Rules 10, 11, 13)
- Not: "Bug was fixed where validation was not working"
- But: "Fix validation in user registration"

- Not: "Updates were made to improve the performance"
- But: "Cache API responses to reduce latency"

### API Documentation (Rule 10: Active Voice)
- Not: "The user object will be returned by this endpoint"
- But: "This endpoint returns the user object"

- Not: "Errors can be handled by catching exceptions"
- But: "Catch exceptions to handle errors"

### Error Messages (Rule 11: Positive Form)
- Not: "Configuration file not found"
- But: "Configuration file missing: /etc/app.conf"

- Not: "Invalid credentials were not accepted"
- But: "Invalid credentials. Check username and password"

### Code Comments (Rule 13: Omit Needless Words)
- Not: "This function is used for the purpose of validating user input"
- But: "Validates user input"

- Not: "In the event that the user is not authenticated"
- But: "If user is unauthenticated"

### Documentation (Rule 12: Concrete Language)
- Not: "The system provides functionality for data management"
- But: "The system stores, retrieves, and updates customer records"

- Not: "Performance improvements were implemented"
- But: "Queries now execute 40% faster"

### Code Placement (Rule 16: Keep Related Words Together)
- Not: "The function only returns data when authenticated"
- But: "The function returns data only when authenticated"

- Not: "We should in the future consider adding this feature"
- But: "We should consider adding this feature in the future"
