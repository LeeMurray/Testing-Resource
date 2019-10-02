# DATA TYPE ATTACK

| Paths/Files                                                   | Time & Date                         | Numbers                     | 
| ------------------------------------------------------------  | ----------------------------------- | --------------------------- | 
| Long Name (>255 Chars)                                        | Timeouts                            | 0                           | 
| Special Characters in Name (Space*?/\|<>,.(){}[]:;"!@#~£$%^&) | Time Difference Between Machines    | Scientific Notation (1E-16) | 
| Non-Existent                                                  | Crossing Time Zones                 | Negative                    | 
| No Space                                                      | Leap Days                           | Floating Point/Decimal      | 
| Minimal Space                                                 | Invalid Days (30th Feb)             | With Commas                 | 
| Write-Protected                                               | Feb 29th (On non leap years)        |                             | 
| Unavailable                                                   | Differnt Formats                    |                             | 
| Locked                                                        | Reset Clocks Backwards and Forwards |                             | 
| On Remote Machine                                             |                                     |                             | 
| Corrupted                                                     |                                     |                             |

| String												| General																							  |
| ----------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
| Long (255, 256 or more)							    | Violates Domain-Specific Rules (an IP Address of 999.999.999.99 an email with no @ and age of -1)	  |
| Accented Chars										| SQL Reserved Words																				  |
| Asian Chars										    | Violates Uniqueness Constraint																	  |
| Common Delimiters & Special Characters				| Passwords Encryted in Configuration Files															  |
| Leave Blank										    |																								      |
| Single Space										    |																									  |
| Multi Space										    |																									  |
| Leading Spaces										|																									  |
| With All Actions (Entering, Searching, Updating etc)  |																									  |
| Max (UI, Scheme & DB)								    |																									  |

---

# WEB TESTING

| Navigation	                                                    |	Input																														 |
| ----------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ |
| Back (Watch for 'Expired' message and double-posted transactions) | HTML/JavaScript Injection (Allowing The User to Enter Arbitrary HTML Tags and JS Commands Can Lead to Security Vulnerabilities)|
| Refresh															| Check Max Length Defined on Text Inputs																						 |
| Bookmark the URL													| > 5000 Chars in Text Areas																									 |
| Select Bookmark When Logged Out									|																																 |
| Hack the URL (Change/Remove Parameters)							|                                   																							 |
| Multi Browser Instance Open										|																																 |

|	Syntax													 |	Preferences	           |
| ---------------------------------------------------------- | ----------------------- |
| [HTML Syntax Checker](http://validator.w3.org/)            | JaveScript Off		   |
| [CSS Syntax Checker] (http://jigsaw.w3.org/css-validator/) | Cookies Off			   |
|															 | Security High		   |
|															 | Resize Browser Window   |
|															 | Change Font Size        |

---

# TESTING WISDOM

* A test is an experiment designed to reveal information or answer a specific question about the software or system.
* Stakeholders have questions; testers have answers
* Don't confuse speed with progress
* Take a contrary approach
* Observation is exploratory
* The narrower the view, the wider the ignorance
* Big bugs are often found by coincidence
* Bugs cluster
* Vary sequences, configurations and data to increase the probability that, if there is a problem, testing will find it
* It's all about the variables

---

# HEURISTICS

| Heuristic         | Description 																																																																																							 |
| ----------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Variable Analysis | Identify anything whose value can change. Variables can be obvious, subtle or hidden.																																																																					 |
| Touch Points		| Identify and public or private interface that provides visibility or control. Provides places to provoke, monitor and verify the system.																																																								 |
| Boundaries		| Approaching the boundary (All most too big, almost too small) at the boundary																																																																							 |
| Goldilocks		| Too Big, Too Small, Just Right																																																																																		 |
| CRUD				| Create, Read, Update, Delete																																																																																			 |
| Follow The Data	| Perform a sequence of actions involving data, verifying the data integrity at each step.(Example: Enter > Search > Report > Export > Import > Update > View)																																																			 |
| Configurations	| Varying the Variables related to configuration (Screen Resolution; Network Speed, Latency, Signal Strength; Memory; Disk Availability  Count heuristic applied to any peripheral such as 0, 1, Many Monitors, Mice, Or Printers)																																		 |
| Interruptions		| Log Off, Shut Down, Reboot, Kill Process, Disconnect, Hibernate, Timeout, Cancel																																																																						 |
| Starvation		| CPU, Memory, Network or Disk at maximum capacity																																																																														 |
| Position			| Beginning, Middle, End (Edit at the beginning of the line, middle of the line, end of the line)																																																																		 |
| Selection			| Some, None, All (Some permissions, No permissions, All permissions)																																																																									 |
| Count				| 0, 1, Many (0 transactions, 1 transactions, Many simultaneous transactions)																																																																							 |
| Multi-User		| Simultaneous create, Update, Delete from two accounts or same account logged in twice																																																																					 |
| Flood				| Multiple simultaneous transactions or requests flooding the queue																																																																										 |
| Dependencies		| Identify 'has a' relationship (A customer has an invoice; an Invoice has multiple line items). Apply CRUD, Count, Position and/or Selection heuristics (Customer has 0, 1, many invoices; Invoice has 0, 1, many line items; Delete last line item then read; Update first line item; Some, None, All line items are taxable; Delete Customer with 0, 1, Many Invoices)|
| Constraints		| Violate constraints (Leave required fields blank, Enter invalid combinations in dependent fields, enter duplicate ID's or Names) Apply with the Input Method heuristic.																																																 |
| Input Method		| Typing, Copy/Paste, Import, Drag/Drop, Various Interfaces (GUI vs API)																																																																								 |
| Sequences			| Vary Order of Operations, Undo/Redo, Reverse, Combine, Invert, Simultaneous																																																																							 |
| Sorting			| Alpha vs Numeric, Across Multiple Pages																																																																																 |
| State Analysis	| Identify states and events/transactions, then represent then in a picture or table. Work with the Sequences and  Interruption heuristic.																																																								 |
| Map Making		| Identify a 'base' or 'home' state. Pick a direction and take one step. Return to base. Repeat.																																																																		 |
| User & Scenarios	| Use Cases, Soap Operas, Personae, Extreme Personalities																																																																												 |

---

# FRAMEWORKS

| Framework 	 | Description  |																																																																	  |
| -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Judgement		 | Inconsistencies, Absences and Extras with respect to Internal, External - Specific, or External - Cultural references points.																																					  |
| Observations	 | Input/Output/Linkage																																																																  |
| Flow			 | Input/Processing/Output																																																															  |
| Requirements	 | User/Functions/Attributes/Constraints																																																											  |
| Nouns & Verbs	 | The object or data in the system and the ways in which the system manipulaites it. Also, adjectives (attributes) such as Visible, Identical, Verbose and Adverbs (action descriptors) such as Quickly, Slowly, Repeatedly, Precisely, Randomly. Good for creating random scenarios |
| Deming's Cycle | Plan, Do, Check, Act																																																																  |

---
