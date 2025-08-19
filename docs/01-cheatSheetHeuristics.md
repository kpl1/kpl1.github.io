# Heuristics

---

### Testing Wisdom
- A test is an experiment designed to reveal information or answer a specific question about the software or system
-  Stakeholders have questions; testers have answers
-  Don’t confuse speed with progress
- Take a contrary approach
- Observation is exploratory
- The narrower the view, the wider the ignorance
- Big bugs are often found by coincidence
- Bugs cluster
- Vary sequences, configurations, and data to increase the probability that, if there is a problem, testing will find it
- It’s all about the variables
- I am not all humans, not everyone does things as I do


## Heuristics lists

| Name | Description |
| :---------------: | :-----|
| Variable Analysis  |   Identify anything whose value can change. Variables can be obvious, or hidden |
| Never and Always  | For example, software should always maintain accurate account balances and never compromise user data. |
| Boundaries  | Approaching the Boundary (almost too big, almost too small), At the Boundary |
| Goldilocks  |   Too Big, Too Small, Just Right   |
|CRUD|  Create, Read, Update, Delete |
| Follow the Data | Perform a sequence of actions involving data, verifying the data integrity at each step.(Example: Enter → Search → Report → Export → Import → Update → View) |
|   Configurations |  Varying the variables related to configuration (Screen Resolution; Network Speed,Latency, Signal Strength; Memory; Disk Availability; Count heuristic applied to any peripheral such as 0, 1, Many Monitors, Mice, or Printers).  |
|  Interruptions  |  Log Off, Shut Down, Reboot, Kill Process, Disconnect, Hibernate, Timeout, Cancel  |
|  Starvation |  CPU, Memory, Network, or Disk at maximum capacity  |
|  Position  |   Beginning, Middle, End (Edit at the beginning of the line, middle of the line, end of the line)  |
|   Selection  |   Some, None, All (Some permissions, No permissions, All permissions)  |
|  Count   |   0, 1, Many (0 transactions, 1 transactions, Many simultaneous transactions) Multi-User Simultaneous create, update, delete from two accounts or same account logged in twice  |
|   Flood  |  ultiple simultaneous transactions or requests flooding the queue - e.g. making/selecting a submit request/button multiple times  |
|   Dependencies  |  Identify “has a” relationships (a Customer has an Invoice; an Invoice has multiple Line Items). Apply CRUD, Count, Position, and/or Selection heuristics (Customer has 0, 1, many Invoices; Invoice has 0, 1, many Line Items; Delete last Line Item then Read; Update first Line Item; Some, None, All Line Items are taxable; Delete Customer with 0, 1, Many Invoices).  |
|  Constraints  |   Violate constraints (leave required fields blank, enter invalid combinations in dependent fields, enter duplicate IDs or names). Apply with the Input Method heuristic.  |
|  Input Method  |  Typing, Copy/Paste, Import, Drag/Drop, Various Interfaces (GUI v. API)  |
|   Sequences  |   Vary Order of Operations → Undo/Redo → Reverse → Combine → Invert → Simultaneous  |
|  Sorting  |  Alpha v. Numeric → Across Multiple Pages  |
|   State Analysis   |  Identify states and events/transitions, then represent them in a picture or table. Works with the Sequences and Interruption heuristics  |
|  RCRCRC (Karen N. Johnson)  |  Recent - what testing around new areas of code should I think about Core - what essential functions or features must continue to work? Risky - what features or areas of code are inherently more risky? Configuration Sensitive - what code is dependent on environment settings? Repaired - what code has changed to address defects and potentially created issues? Chronic - what code typically breaks features that need to be tested?  |
|   FAILURE (Ben Simo)  |   Functional, Appropriate, Impact, Log, UI, Recovery, Emotions  |
|  WWWWWHKE  (sounds like “wiki”(Darren McMillan)) |  Who is this for? What is this for? When & by whom is it to be done? Where is it being done? Why is it being done? How is it being achieved? What questions does my Knowledge & Experience produce?  |
|  Combat Bias with Heuristics of Diversity (Ash Coleman)  |   Does this work for me? Does this work for them? Does this work for someone I have never considered or ever met?  |
|  Seven Dwarfs (Cassandra H. Leung)  |   Grumpy, Happy, Sleepy, Bashful, Sneezy, Dopey, and Doc  |
|   Specs/Designs Watchlist (Gerard McCann) |   Ambiguity, weasel words (like could, should or may), Fudge (e.g. statements like ‘this will be resolved at a later date’, but no specifics around who and when), Confusing terminology, jargon or obscure acronyms, Oversimplification, Overcomplication. |
|  TORCH  (Simon Tomes)     |  Timer, Oracles, Risks, Consider these questions, Heuristics.  |
|  MCOASTER  (Michael Kelly) |   Mission, Coverage, Obstacles, Audience, Status, Techniques. Environment, Risk   |
|  Seen and Heard  (Ady Stokes)  |  For everything you can see, is it announced by a screen reader? For everything you hear, can it be read (transcript, subtitles, captions, audio descriptions)  |
|  TuTTu and TaTTa (Mark Winteringham)  |   Testing the UI or Testing Through the UI - Testing the API or Testing Through the API  |
|  SACRED (Richard Bradshaw) |  State Management, Actions, Codified Oracle, Reporting, Execution, Deterministic  |
|   TRIMS (Richard Bradshaw) |  Targeted, Reliable, Informative, Maintainable, Speedy |



### References
1. [Test Heuristics Cheat Sheet ](https://www.ministryoftesting.com/articles/test-heuristics-cheat-sheet) by Simon Tomes
1. [Test Heuristics Cheat Sheet ](https://bbst.courses/elisabeth-hendrickson-james-lyndsay-and-dale-emery-test-heuristics-cheat-sheet/) by Elisabeth Hendrickson, James Lyndsay, and Dale Emery
1. [Software Testing Heuristics and mnemonics](https://ladyogitakailas.medium.com/software-testing-heuristics-and-mnemonics-26eeb9a6f3ac) by 
Yogita kailas lad
