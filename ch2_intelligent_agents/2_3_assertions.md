# 2.3
29.06.2020.

 For each of the following assertions, say whether it is true or false and support your answer with examples or counterexamples where appropriate.

### a. An agent that senses only partial information about the state cannot be perfectly rational.

A: False. If the extra information about the state that the agent does not know is not needed to make a rational decision then the agent can be perfectly rational. For example an autonomous vehicle will drive just as well if it doesn't know the current position of Jupyter in the sky.

S: False. Perfect rationality refers to the ability to make good decisions given the sensor
information received.

---

### b. There exist task environments in which no pure reflex agent can behave rationally.

A: Yes, they do exist. A pure reflex agent can't by definition behave rationally if it needs to know some previous percept, because it is not allowed to store state, so we just need a task environment with an external environment that's state is heavily dependent on previous states. The same autonomous vehicle example works- if the agent is not allowed to store state about the positions of objects, it cannot determine their velocities, so forgoing inconcievably fast sensors, processors and actuators, the vehicle would crash.

S: True. A pure reflex agent ignores previous percepts, so cannot obtain an optimal state
estimate in a partially observable environment. For example, correspondence chess is
played by sending moves; if the other player’s move is the current percept, a reflex agent
could not keep track of the board state and would have to respond to, say, “a4” in the
same way regardless of the position in which it was played.

---

### c. There exists a task environment in which every agent is rational.

A: Yes. A task environment with a static performance measure.

S: True. For example, in an environment with a single state, such that all actions have the
same reward, it doesn’t matter which action is taken. More generally, any environment
that is reward-invariant under permutation of the actions will satisfy this property.

---

### d. The input to an agent program is the same as the input to the agent function.

A: No, input to an agent function is all possible percept sequences, but to a program- only one.

S: False. The agent function, notionally speaking, takes as input the entire percept sequence up to that point, whereas the agent program takes the current percept only.

---

### e. Every agent function is implementable by some program/machine combination.

A: It is not. An action in an agent function can be unimplementable, making the function unimplementable also. For example: if square A is clean, go to square B at a speed faster than c.

S: False. For example, the environment may contain Turing machines and input tapes and
the agent’s job is to solve the halting problem; there is an agent function that specifies
the right answers, but no agent program can implement it. Another example would be
an agent function that requires solving intractable problem instances of arbitrary size in
constant time.

---

### f. Suppose an agent selects its action uniformly at random from the set of possible actions. There exists a deterministic task environment in which this agent is rational.

A: Yes, if size of the set of possible actions is 1 or all possible actions make the agent equally rational.

S: True. This is a special case of (c); if it doesn’t matter which action you take, selecting
randomly is rational.

---

### g. It is possible for a given agent to be perfectly rational in two distinct task environments.

A: Well what does it mean for task environments to be distinct? Agents and task environments have common parts: actuators and sensors, so an argument could be made that two distinct task environments cannot have the same agent. If some overlap is allowed though, I think it is possible: the agent just has to be able to adapt- humans can be such an agent, though rarely perfectly rational.

S: True. For example, we can arbitrarily modify the parts of the environment that are
unreachable by any optimal policy as long as they stay unreachable.

---

### h. Every agent is rational in an unobservable environment.

A: Unobservable environment means no percept sequence, so the agent can only rely on built-in knowledge. The definition of a rational agent seems lacking for this application, but given what it says, the statement is true.

S: False. Some actions are stupid—and the agent may know this if it has a model of the
environment—even if one cannot perceive the environment state.

---

### i. A perfectly rational poker-playing agent never loses.

A: False. A perfectly rational poker agent loses, just less on average than non-perfect agents. Since probabilities are involved, the superior rationality of this perfect agent can only be seen over many games.

S: False. Unless it draws the perfect hand, the agent can always lose if an opponent has
better cards. This can happen for game after game. The correct statement is that the
agent’s expected winnings are nonnegative.

---
