# 1.10
28.06.2020.

Q: Is AI a science, or is it engineering? Or neither or both? Explain.

A: It can be at least one or both. In academia AI is mostly science, but engineering is still needed. In industry it is mostly engineering but science can still be needed to solve problems closer to the edge. I don't see how it could be neither.

---

S: This question is intended to be about the essential nature of the AI problem and what is
required to solve it, but could also be interpreted as a sociological question about the current
practice of AI research.
A science is a field of study that leads to the acquisition of empirical knowledge by the
scientific method, which involves falsifiable hypotheses about what is. A pure engineering
field can be thought of as taking a fixed base of empirical knowledge and using it to solve
problems of interest to society. Of course, engineers do bits of science—e.g., they measure the
properties of building materials—and scientists do bits of engineering to create new devices
and so on.
As described in Section 1.1, the “human” side of AI is clearly an empirical science—
called cognitive science these days—because it involves psychological experiments designed
out to find out how human cognition actually works. What about the the “rational” side?
If we view it as studying the abstract relationship among an arbitrary task environment, a
computing device, and the program for that computing device that yields the best performance
in the task environment, then the rational side of AI is really mathematics and engineering;
it does not require any empirical knowledge about the actual world—and the actual task
environment—that we inhabit; that a given program will do well in a given environment is a
theorem. (The same is true of pure decision theory.) In practice, however, we are interested
in task environments that do approximate the actual world, so even the rational side of AI
involves finding out what the actual world is like. For example, in studying rational agents
that communicate, we are interested in task environments that contain humans, so we have
to find out what human language is like. In studying perception, we tend to focus on sensors
such as cameras that extract useful information from the actual world. (In a world without
light, cameras wouldn’t be much use.) Moreover, to design vision algorithms that are good
at extracting information from camera images, we need to understand the actual world that
generates those images. Obtaining the required understanding of scene characteristics, object
types, surface markings, and so on is a quite different kind of science from ordinary physics,
chemistry, biology, and so on, but it is still science.
In summary, AI is definitely engineering but it would not be especially useful to us if it
were not also an empirical science concerned with those aspects of the real world that affect
the design of intelligent systems for that world.