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
  ```
  I used Microsoft Copilot
  ```
- Give one example of an AI suggestion that was correct (including what the AI suggested and how you verified the result).
  ```
  The Copilot suggested me to change the logic of the hint (from 'HIGHER' to 'LOWER' and opposite). I verified by reading the code one more time. It's a little bit hard to compare the original code and new code since they come after the original code. After apply it, I ran the code one more time and play it again to see if it is finalized.
  ```
- Give one example of an AI suggestion that was incorrect or misleading (including what the AI suggested and how you verified the result).
  ```
  There is the one that I still haven't fixed yet. That is the Developer Debug Info box. I told the AI about the problem of not synchronized info for the attemps and system of counting and decreasing points, which made me confused. After describing the problem to the Copilot, it misundertood and create one copy of that box to update right after each time the player submit. That's not what I mean. And I knew there was something wrong by read the fixed code again before run it. I then ran the app to really confirm my understanding about Copilot's miunderstanding and it shows that I was right.
  ```
---

## 3. Debugging and testing your fixes

- How did you decide whether a bug was really fixed?
  ```
  To check if the bug was really fixed, I read the logic, traced how the functions work and if the functions were well imported, then compared the conditions with the assumptions and tested the app again (playing multiple times).
  ```
- Describe at least one test you ran (manual or using pytest)  
  and what it showed you about your code.
  ```
  One test that I ran after fixing the code is the point systems (hint and developer debug info for each difficulty level). And it showed that I have sucessfully fixed the logic mistake of the code.
  ```
- Did AI help you design or understand any tests? How?
  ```
  The AI helped me so much in finding the spot of the bug in the code or the problem that I want to find in the bug. Then it shows me the suggestion for the change. I then just need to read the code again and apply it.
  ```
---

## 4. What did you learn about Streamlit and state?

- How would you explain Streamlit "reruns" and session state to a friend who has never used Streamlit?
  ```
  Streamlit "reruns" run the script from top-to-bottom on every user action, and Streamlit sends updated interface to browser. Session state is a place to store data across those runs.
  ```
---

## 5. Looking ahead: your developer habits

- What is one habit or strategy from this project that you want to reuse in future labs or projects?
  - This could be a testing habit, a prompting strategy, or a way you used Git.
  ```
  One habit or strategy that I want to reuse in the future labs or projects are checking the logic of the code before run the app for testing. It helps me understand what AI will do in the future and shorten my testing time since I just usually check for the edge cases more than usual cases that can happen.
  ```
- What is one thing you would do differently next time you work with AI on a coding task?
  ```
  I will try to explain the context and tasks that the AI has to do as detailed as possible so that the Ai can help me follow the idea and abstract (clear enough to understand).
  ```
- In one or two sentences, describe how this project changed the way you think about AI generated code.
  ```
  This project changed my thinking about AI from something as super power and can alter human force in the future to a supporter and can accompany with me in the future and promote my standing in programming.
  ```
