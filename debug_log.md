# Debug Log

**Explain how you used the VSCode debugger tools to uncover the bugs in Exercise 7. Be specific. What breakpoints did you set? Where did you step to? What made you realize the error?**

_Example: I set a breakpoint on line 5 and stepped until line 12. There, I discovered that the `x` variable had a value of `-3`, whereas it should have had a value of `7`. That made me realize that we should be adding the two numbers `x` and `y`, instead of subtracting._

1. first i set a breakpoint at line5
1. i realized that for the second loop around, sentence was cleared out using continue
1. i then stepped over the code and the problem was that remainder_of_sentence was replacing sentence in the recursive loop and it's value was empty.
1. after a slight lookaround the reason why remainder_of_sentence was clear is because it was taking the "remainder" of start_string rather than the remainder of the... well... sentence. start_string => sentence
1. after the start_string fix, i reran the code, stepping over from line5 and caught another problem at line 13 where the next iteration wasnt the remainding of the sentence but... the start string?!?! start_string => sentence
1. it works... it fixed... good nite