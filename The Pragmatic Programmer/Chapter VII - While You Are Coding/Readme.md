# Chapter VII - While You Are Coding:

- Conventional wisdom says that once a project is in the coding phase, the work is mostly mechanical, transcribing the design into executable statements. We think that this attitude is the single biggest reason that software projects fail.
- Coding is not mechanical, otherwise programmers would've been largely redundant from long ago.
- Pragmatic Programmers think critically about all code, including our own.
- Testing is not about finding bugs, it’s about getting feedback on your code.
- The major benefits of testing happen when you think about and write the tests, not just when you run them.
- Listen to your instincts. Instincts are simply a response to patterns packed into our nonconscious brain.
- Listening to your instincts doesn’t mean you can just fly on autopilot either.
- The trick is first to notice your instinct is happening, and then to work out why.
- Everyone fears the empty screen, the lonely blinking cursor surrounded by a whole bunch of nothing.
- Sometimes code just flies from your brain into the editor: ideas become bits with seemingly no effort. Other days, coding feels like walking uphill in mud.
- Your code is trying to tell you something. It’s saying that this is harder than it should be.
- Give yourself a little time and space to let your brain organize itself. Stop thinking about the code, and do something that is fairly mindless, away from a keyboard.
- If that’s not working, try externalizing the issue. Make doodles about the code you’re writing, or explain it to a coworker. Or to
  your rubber duck.
- The authors found a brain hack that seems to work: tell yourself you need to prototype something.

---

### Do the following:

- [x] **1.** Write “I’m prototyping” on a sticky note, and stick it on the side of your screen.
- [x] **2.** Remind yourself that prototypes are meant to fail. And remind yourself that prototypes get thrown away, even if they don’t fail. There is no downside to doing this.
- [x] **3.** In your empty editor buffer, create a comment describing in one sentence what you want to learn or do.
- [x] **4.** Start coding.

If you start to have doubts, look at the sticky note. At some point during the first prototype you will be surprised to find yourself humming along with your music, enjoying the feeling of creating code. Afterwards delete all the prototype code, throw away the sticky note, and fill that empty editor buffer with bright, shiny new code.

---

- As a programmer you will deal with code made by different people. That means that they will make decisions in a different way for different reasons. Not worse, just different.
- When you spot things done in a way that seems strange, jot it down.
- Look for patterns. If you can see what drove them to write code that way, you may find that the job of understanding it becomes a lot easier.
- We should avoid programming by coincidence—relying on luck and accidental successes—in favor of programming deliberately.
- Sometimes it can be pretty easy to confuse a happy coincidence with a purposeful plan.
- Human beings are designed to see patterns and causes, even when it’s just a coincidence.
- Tests that seem to pass on your machine but not on the server might indicate a difference between the two environments, or maybe it’s just a coincidence. Don’t assume it, prove it.
- Finding an answer that happens to fit is not the same as finding the right answer.
- Assumptions that aren’t based on well-established facts are the bane of all projects.
- Don’t code in the dark. Build an application you don’t fully grasp, or use a technology you don’t understand, and you’ll likely be bitten by coincidences.
- Rely only on reliable things.
- Don’t just test your code, but test your assumptions as well. Don’t guess; actually try it.
- Don’t be a slave to history. Don’t let existing code dictate future code.
- As a program evolves, it will become necessary to rethink earlier decisions and rework portions of the code.
- Software is like gardening - it is more organic than concrete. You plant many things in a garden according to an initial plan and conditions.
- Refactoring is a disciplined technique for restructuring an existing body of code, altering its internal structure without changing its external behavior.
- Refactoring is a day-to-day activity, taking low-risk small steps, more like weeding and raking.
- You refactor when you’ve learned something; when you understand something better than you did last year, yesterday, or even just ten minutes ago.
- Refactoring your code—moving functionality around and updating earlier decisions—is really an exercise in pain management.
- Refactoring, as with most things, is easier to do while the issues are small, as an ongoing activity while coding.
- Refactoring is an activity that needs to be undertaken slowly, deliberately, and carefully.

---

### How to refactor without doing more harm than good:

- [x] **1.** Don’t try to refactor and add functionality at the same time.
- [x] **2.** Make sure you have good tests before you begin refactoring. Run the tests as often as possible. That way you will know quickly if your changes have broken anything.
- [x] **3.** Take short, deliberate steps: move a field from one class to another, split a method, rename a variable. Refactoring often involves making many localized changes that result in a larger-scale change. If you keep your steps small, and test after each step, you will avoid prolonged debugging.

---

- A test is the first user of your code.
- If you do TDD, don’t forget to stop every now and then and look at the big picture. It is easy to become seduced by the green "tests passed" message.
- Tests can definitely help drive development. But, as with every drive, unless you have a destination in mind, you can end up going in circles.
- Like our hardware colleagues, we need to build testability into the software from the very beginning, and test each piece thoroughly before trying to wire them together. Unit testing.
- We want to avoid creating a “time bomb”—something that sits around unnoticed and blows up at an awkward moment later in the project.
- All software you write will be tested—if not by you and your team, then by the eventual users—so you might as well plan on testing it thoroughly.
- A culture of testing means all the tests pass all the time.
- Security through obscurity just doesn’t work.

---

### Security Principles:

- [x] **1.** Minimize Attack Surface Area
- [x] **2.** Principle of Least Privilege
- [x] **3.** Secure Defaults
- [x] **4.** Encrypt Sensitive Data
- [x] **5.** Maintain Security Updates

---

- Use the least amount of privilege for the shortest time you can get away with.
- It's better to let each individual decide for themselves the trade-offs between security and convenience. That's why defaults should be tight.
- Don’t leave personally identifiable information, financial data, passwords, or other credentials in plain text, whether in a database or some other external file. That point is especially important given the amount of tools that have surfaced right here on Github that analyze repos and find exposed channels of entry by the thousands per day.
- Don’t check in secrets, API keys, SSH keys, encryption passwords or other credentials alongside your source code in version control.
- Apply security patches quickly.
- What’s in a name? When we’re programming, the answer is “everything!”
- Things should be named according to the role they play in your code.
- Consider having a a project glossary, listing the terms that have special meaning to the team.
- Name well; rename well when needed.
