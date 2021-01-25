# Chapter 4 - Pragmatic Paranoia:

- You can't write perfect software and that shouldn't hurt, it doesn't exist.
- Build in defenses against your own mistakes.

---

### Design By Contract:

A program that meets the requirements of being DBC or Design By Contract must meet 3 conditions:

- [ ] **Preconditions:** What must be true in order for a routine to be called. Basically a call's requirements.
- [ ] **Postconditions:** What the routine is guaranteed to get done and the state of the world when it is finished.
- [ ] **Class Invariants:** A class which ensures that this condition is always true from the point of view of a caller.

The aim is for the Contract to become a routine. Some languages better support this concept like Clojure and Elixir, for example.

A more elaborate description can be found in this video: https://www.youtube.com/watch?v=aA29jZYdJos

---

- Be strict in what your code will accept and make it promise as little as possible in return.
- DBC and TDD (Test-Driven Development) are different tools appropriate for different jobs.
- The folly of TDD is that it concentrates on a "happy path" or an idealized version of consequences.
- Don't fall prey to the "it can't happen mentality"
- When error messages show their head, it means something has gone wrong in our processes of defensive programming
- Read the error message - don't ignore it.
- When your code discovers something that was supposed to be impossible, your program is no longer viable.
- Anything from that point forward "working" should be suspect.
- Self-deception is particularly prevalent in programming circles.
- Assertions check for things that should never happen. An integer being a negative would be an example.
- Assertions can serve as a way to catch "impossible" situations from happening.
- Make sure your assertions, which can have side effects, are under control. Fix issues, don't add to them.
- Assertions are seen as unnecessary overhead after testing. Not so, leave them turned on.
- The reasons are because testing does not find all bugs and our programs live in a dangerous world.
- Resource management can be tedious, but it's a necessary part of being a Pragmatic Programmer.
- Finish what you start, make sure the resources you allocate to a function are properly deallocated once it's finished.
- When in doubt, it always pays to reduce scope.
- Deallocate resources in the opposite order in which you allocate them.
- Another good idea is to use a "finally" clause in your code if the language allows it.
- Always take small steps. Be deliberate, check for feedback and adjust. "Don't outrun your headlights."
- Tasks that require "fortune telling" are too big. Cut them down to be manageable and don't engage in wild speculation.
- Often tomorrow looks like today. But don't count on it.
