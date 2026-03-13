# 💭 Reflection: Game Glitch Investigator

Answer each question in 3 to 5 sentences. Be specific and honest about what actually happened while you worked. This is about your process, not trying to sound perfect.

## 1. What was broken when you started?

- What did the game look like the first time you ran it?
  ```
  I can see that the UI is quite simple, easy to understand. However, there is the developer debug info box that shouldn't be shown to the player. The instruction is direct, clear; however, it still doesn't show how to play the game for the newbie. For example, there is no instruction to put the number to the box, maybe because the UI is too simple and cannot get the attraction of the player to the answer box.
  ```
- List at least two concrete bugs you noticed at the start  
  (for example: "the hints were backwards").
  ```
  The game take the string as one time input although it is illegal. I expected that it still warning but won't take off 1 attempt from player.
  The hint should show lower instead of higher and higher instead of lower.
  The attempts are counting wrong, while the blue box show that I have 1 attempt left, the result showed and said out of attempt. I expected them to be synchronized and show the same number.
  The history should take the guess right away instead of getting it after the player next guess. I think that's the reason why the attempt counter has problems.
  The New Game button doesn't work. When I hit the new game button, only the attempt counter is changed and the counter also wrong.
  Easy mode have less attempts than normal mode and the range of the secrete number is not consistent for all mode. The point is count differently and wrong by each difficulty. I expected it will show points -5 or at least show the highest point ( and it should be 100 instead of 70), then decrease the point right after when the player guess wrong.
  ```
---

## 2. How did you use AI as a teammate?

- Which AI tools did you use on this project (for example: ChatGPT, Gemini, Copilot)?
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).

---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
- Did AI help you design or understand any tests? How?

---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?

---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
- What is one thing you would do differently next time you work with AI on a coding task?
- In one or two sentences, describe how this project changed the way you think about AI generated code.
