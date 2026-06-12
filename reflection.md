# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").

**Bug Reproduction Log**

Document at least 3 bugs you found. Add rows as needed.

| Input | Expected Behavior | Actual Behavior | Console Output / Error |
|-------|-------------------|-----------------|------------------------|
|guess of 41 |correct |correct  |final score of 70 with 1 attempt  |
|started a new game  | ability to play |not able to play  |generated a new secret, attempts is 0, score is 70, history of my previous attempt is there. Issue comes when I enter the secret number into the answer field the game tells me i already won and need to generate a new game. it also stopped generating this message after a while. now anytime i start a new game and enter a number the game doesn't process my input.  |
|guess of 54 |wrong , go higher  |wrong, go lower  |go lower |
|change dfficulty | suggest and accept numbers within difficulty range | number range remains the same |
| attempt | history count of 1 | history count of 0  | |

---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)? Claude 
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result). Claude did not fix any of the issues I mentioned on the first attempt. 
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result). I mentioned the go higher issue as well as the difficulty range. Claude said it was fixed so I copied the code into the file and ran it. The errors remained the same, as if I never spoke to Claude about it. I had the same issue with reporting the intial attempt as 1 instead of 0. Claude said the new code is fixed and addresses this issue as well, but that was not the case either. 

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed? if it functioned in the intended way 
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code. I did manual testing where I switched the difficulty modes, I entered numbers lower and higher than the secret number. It honestly just showed me not to blindly trust AI when coding/completing projects. 
- Did AI help you design or understand any tests? How? no 

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit? Every time something happens on the page, Streamlit reruns your whole script from scratch. Regular variables reset, so anything you want to survive between those reruns — a score, a username, whether a game is over —would be stored in session_state, which is just a dictionary that sticks around for the life of the user's browser session.

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects? I definitely have lost complete trust of AI when coding, but I am also going to apply this to every aspect I use Ai for. Definitely not trusting it without reviewing. 
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task? I think I would focus more on developing the code myself and use AI if I am stuck to gather more information on a topic or a bug I am encountering. 
- In one or two sentences, describe how this project changed the way you think about AI generated code. It has changed the way I think about AI generated code drastically. I don't trust it at all anymore. I don't feel like AI is reliable, not event to a small degree. Instead, I feel like it creates more work rather than lessening the load, which is what we mainly use AI for. 
