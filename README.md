# Where is the Math in: Molecular Vibrations?
## About Me
My name is Daniel Gonzalez. I am currently studying for a Bachelor of Science in Chemistry with minors in Mathematics and Biological Sciences. Although I initially started as a Biology student, it was during my mathematical courses and my time conducting chemistry research that I fell in love with the abstract worlds of Mathematics and Chemistry. During this time, I began taking more math courses and changed my major to Chemistry; up to now, I have covered the following courses:

- Calculus I
- Calculus II
- Calculus III
- Linear Algebra
- Mathematical Modeling (currently)

While also taking more theoretical courses in Chemistry, such as Descriptive Inorganic Chemistry and Spectroscopy. During these courses, I was able to find applications for the math courses I had taken, and where my interest in theoretical chemistry began. With support from Dr. Jesus Alberto Lopez Dominguez, we began to explore ideas to work on a project regarding molecular vibrations. 

## What are Molecular Vibrations?
The following two videos can help give an initial or a deeper understanding of the topic, as you choose.

- [Shorter Video](https://www.youtube.com/watch?v=DJI518yTr2c)
- [More In-Depth Video](https://www.youtube.com/watch?v=Ha5yWbxOqFk&t=368s)

Alternatively, you can check out my video on the subject which covers the content presented in this section:

[![personal_video](http://img.youtube.com/vi/YEDhi-Hszz4/0.jpg)](https://youtu.be/YEDhi-Hszz4)

### Motion in Molecules
The way atoms or molecules "move" can be simplified or expressed through three main ways:
1. Translation
2. Rotation
3. Vibration

In more general terms, for any displacement in three dimensions, atoms exhibit 3 degrees of freedom. Each atom in a molecule will add 3 degrees of freedom to the overall displacement of the molecule giving us a total amount of displacements a molecule can have as:

$$3N$$

where N = # of atoms in the molecule.

In our three axis system, any molecule will use three degrees of freedom to move along the axis (translation) and three to rotate around an axis (rotation). This means that we have $3N-6$ remaining degrees of freedom. If our molecule is linear, meaning rotation along one axis effectively does nothing, then we have $3N-5$ remaining degrees of freedom.

![linear molecule](images\linear_molecule.png) ![nonlinear molecule](images\nonlinear_molecule.png)

These remaining degrees of displacement freedom will contribute to the vibrational motion of a molecule. For non-chemists, another way to think of it is that the degrees of freedom will describe ways in which a molecule can store kinetic energy.

You can describe all motion in a molecule through what are known as normal modes. If you have taken linear algebra, you can relate this to the basis of a vector space. Any type of motion in a molecule can be described as a combination of the normal modes, and the normal modes cannot form each other.


### Bonds as Harmonic Oscillators

We can create an initial approximation by considering bonds and atoms as objects on springs, using equations for what are known as simple harmonic oscillators.

We can derive the equation for any classical simple harmonic oscillator through the use of differential equations as is shown in [Hands On: Simple Harmonic Oscillator](hands-on/1_harmonic_oscillator.md).

### Applying Quantum Behavior (WIP)
We must remember though, that in the world of subatomic particles, classical mechanics stops describing the physical properties and behavior of objects. We must instead turn to Quantum Mechanics.

It was Einstein who first proposed a quantized model of the harmonic oscillator to describe the heat capacity of solids.

$$E = \hslash \omega \left(n + \frac{1}{2}\right)$$

If you know German, you can read [Eintein's original paper on this.](https://doi.org/10.1002/andp.19063270110)

A future addition will be the derivation of the quantum harmonic oscillator using Schrodinger's equation at [Hands On: Quantum Harmonic Oscillator](hands-on\2_quantum_harmonic_oscillator.md).

### Why Study Vibrations?
Vibrations can tell us a lot of information about the molecule. Beginning through IR and Raman spectroscopy, which allow for molecular fingerprinting, detecting groups within a molecule by the wavelengths of light that are absorbed to excite vibrational states. Vibrations, by describing bonds, also describe the strength and type of bonds existing within molecules, which can be useful to predict reactivity. A study of thermodynamics could use molecular vibrations, as Einstein did originally.

## Summary and Conclusions

## References

