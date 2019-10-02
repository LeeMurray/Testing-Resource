# Data Type Attacks
| Paths/Files                                                   | Time & Date                         | Numbers                     | String												|
| ------------------------------------------------------------  | :---------------------------------: | :-------------------------: | :---------------------------------------------------: |
| Long Name (>255 Chars)                                        | Timeouts                            | 0                           | Long (255, 256 or more)								|
| Special Characters in Name (Space*?/\|<>,.(){}[]:;"!@#~£$%^&) | Time Difference Between Machines    | Scientific Notation (1E-16) | Accented Chars										|
| Non-Existent                                                  | Crossing Time Zones                 | Negative                    | Asian Chars											|
| No Space                                                      | Leap Days                           | Floating Point/Decimal      | Common Delimiters & Special Characters				|
| Minimal Space                                                 | Invalid Days (30th Feb)             | With Commas                 | Leave Blank											|
| Write-Protected                                               | Feb 29th (On non leap years)        |                             | Single Space											|
| Unavailable                                                   | Differnt Formats                    |                             | Multi Space											|
| Locked                                                        | Reset Clocks Backwards and Forwards |                             | Leading Spaces										|
| On Remote Machine                                             |                                     |                             | With All Actions (Entering, Searching, Updating etc)	|
| Corrupted                                                     |                                     |                             | Max (UI, Scheme & DB)									|

 General																							|
 -------------------------------------------------------------------------------------------------:	|
 Violates Domain-Specific Rules (an IP Address of 999.999.999.99 an email with no @ and age of -1)	|
 SQL Reserved Words																					|
 Violates Uniqueness Constraint																		|
 Passwords Encryted in Configuration Files															|
																									|
																									|
																									|
																									|
																									|
																									|