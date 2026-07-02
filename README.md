ADA/SPARK 

procedure to_lower_string with spark_mode => On;

Summary of SPARK analysis
=========================

---------------------------------------------------------------------------------------------
SPARK Analysis results        Total       Flow   CodePeer      Provers   Justified   Unproved
---------------------------------------------------------------------------------------------
Data Dependencies                 1          1          .            .           .          .
Flow Dependencies                 1          1          .            .           .          .
Initialization                    1          1          .            .           .          .
Non-Aliasing                      .          .          .            .           .          .
Run-time Checks                  18          .          .    18 (CVC4)           .          .
Assertions                        6          .          .     6 (CVC4)           .          .
Functional Contracts              1          .          .     1 (CVC4)           .          .
LSP Verification                  .          .          .            .           .          .
Termination                       1          .          .     1 (CVC4)           .          .
Concurrency                       .          .          .            .           .          .
---------------------------------------------------------------------------------------------
Total                            29    3 (10%)          .     26 (90%)           .          .


max steps used for successful proof: 1

Analyzed 1 unit
in unit black_list_pswd, 1 subprograms and packages out of 1 analyzed
  black_list_pswd.To_Lower_Internal at black_list_pswd.adb:9 flow analyzed (0 errors, 0 checks and 0 warnings) and proved (26 checks)
  
