# Hint 4

The previous attempts all returned very quickly. Annoyingly quickly. This is because the regex engine matches the first possible way to accept the set of characters and returns. The content string we have provided matches straight away. A ReDoS occurs when we can get the regex engine into a state that it backtracks through many possibilities before returning to say it cannot match the provided string. Try to alter your content string to achieve this state, aka catastrophic backtracking.
