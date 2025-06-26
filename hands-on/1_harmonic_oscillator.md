# The Simple Harmonic Oscillator: Initial Conditions
Solution was obtained from the [Santa Cruz Institute for Particle Physics](https://scipp.ucsc.edu/~haber/ph5B/sho09.pdf)[^1].

Considering an ideal, frictionless, mass-spring system. We can follow the following equations:

**Hooke's Law**

$$F=-kx$$

Where:
- $F =$ force
- $k=$ spring constant
- $x =$ is the position of the object.

![hookelaw](https://math.libretexts.org/@api/deki/files/80489/clipboard_e667a8a3589f79037977e9f590a0856b8.png?revision=1)[^2]

**Angular Frequency of a Massless Spring**

$$\omega = \sqrt{\frac{k}{m}}$$

**Newton's Second Law**

$$F=ma$$

but  $a = \frac{\mathrm d^2}{\mathrm d t^2}x$

**The Derivation**

$$m\frac{\mathrm d^2}{\mathrm d t^2}x = -kx$$

$$m\frac{\mathrm d^2}{\mathrm d t^2}x + kx = 0$$

$$\frac{m}{m}\frac{\mathrm d^2}{\mathrm d t^2}x + \frac{k}{m}x = 0$$

but $\omega = \sqrt{\frac{k}{m}}$

$$\frac{\mathrm d^2}{\mathrm d t^2}x + \omega^2x = 0$$

or

$$\frac{\mathrm d^2}{\mathrm d t^2}x + = -\omega^2x$$ 

We now have what is considered a second-order differential equation. We can remember that harmonic oscillatory motion is periodic, following a sinusoidal pattern, so we can give an initial guess of our function based on sine and cosine functions. Before that, let us set some initial conditions.

At time = 0, what we will say is the following: $x(t)=x_{0}$ and $\frac{\mathrm d}{\mathrm dt}x(t)=v_{0}$. Which is saying that at time = 0, our position will be $x_{0}$, any initial position, and our velocity will be $v_{0}$, any initial velocity. 

Let's try to come up with a solution to solve our first initial condition. What we want is for our function to be $x_{0}$ or a value that maintains $x_{0}$ as itself.

When $t = 0$:

$$\cos (0) = 1$$

So maybe,

$$x(t)= x_{0}\cos (t)$$

$$x(0) = x_{0}(1) = x_{0}$$

Now let's try and solve for our second condition by taking this derivative.

$$\frac{\mathrm d}{\mathrm d t}x(t) = -x_{0}\sin (t)$$

If we were to substitute $t=0$ here, we would get 0, which is an assumption that we do not have an initial velocity. But that's a specific answer; we need a generalization.

So if we know that $\cos (0) = 1$, could we do something similar to the first case? If we want to get $v_{0}$ from our first derivative, we need to add a function that, when differentiated, turns into a cosine.

$$x(t) = x_{0}\cos (t) + v_{0}\sin (t)$$

And this still holds for our initial conditions.

A final test would be to get the second derivative to test if it complies with $\frac{\mathrm d^2}{\mathrm d t^2}x(t) + = -\omega^2x(t)$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -x_{0}\cos (t) - v_{0}\sin (t)$$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -1(x_{0}\cos (t) + v_{0}\sin (t))$$

but $x_{0}\cos (t) + v_{0}\sin (t) = x(t)$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -1(x(t))$$

Hmm, not quite what we wanted, but really close, all that we are missing is to multiply all of this by $\omega^2$ for this to hold true. This is a simple fix; we can place our constant $\omega$ in a place where it will not modify our initial conditions, such as inside the trigonometric functions.

$$x(t) = x_{0}\cos (\omega t) + v_{0}\sin (\omega t)$$

But let's test it!

$$\frac{\mathrm d}{\mathrm d t}x(t) = -x_{0}\omega \sin (\omega t) + v_{0} \omega \cos (\omega t)$$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -x_{0}\omega^2 \cos (\omega t) - v_{0} \omega^2 \sin (\omega t)$$

Which does comply with our differential equation, but if we test our initial conditions, particularly velocity, we'll see it no longer holds there.

$$\frac{\mathrm d}{\mathrm d t}x(0) = -x_{0}\omega \sin (\omega (0)) + v_{0} \omega \cos (\omega (0))$$

$$\frac{\mathrm d}{\mathrm d t}x(t) = 0 + v_{0} \omega (1)$$

Thankfully, this is an easy solution, by simply changing our function so that instead of just $v_{0}$, we can put $\frac{v_{0}}{\omega}$, quickly solving this issue.

$$x(t) = x_{0}\cos (\omega t) + \frac{v_{0}}{\omega}\sin (\omega t)$$

$$\frac{\mathrm d}{\mathrm d t}x(t) = -x_{0}\omega \sin (\omega t) + v_{0} \cos (\omega t)$$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -x_{0}\omega^2 \cos (\omega t) - v_{0} \omega \sin (\omega t)$$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -\omega^2(x_{0}\cos (\omega t) + \frac{v_{0}}{\omega} \sin (\omega t))$$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -\omega^2(x(t))$$

**Harmonic Oscillator Based on Amplitude and Phase Change**

The principal equation describing a harmonic oscillator assumes no initial conditions. We have our second-order differential equation obtained through Hooke's Law and Newton's second law of motion.

$$\frac{\mathrm d^2}{\mathrm d t^2}x + \omega^2x = 0$$

$$\frac{\mathrm d^2}{\mathrm d t^2}x = -\omega^2x$$

If we want a more general solution, we can start by asking ourselves what type of function, when derived, is itself times a constant. From our knowledge of Calculus, we can immediately say that an exponential function of the form:

$$x(t) = e^{rt}$$

Where r is any arbitrary constant. If we assume this, we can place this function into the equation we obtained before:

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = r^2 e^{rt}$$

$$r^2 e^{rt} + \omega^2e^{rt} = 0$$

We know that any exponential function cannot be 0, so we need to solve for the value of our constants that makes this equation equal to 0.

We can find our arbitrary constant r by solving the following equation:

$$(r^2 + \omega^2) = 0$$

$$r^2 = -\omega^2$$

$$\sqrt{r^2} = \sqrt{-\omega^2}$$

$$r = \pm i \omega$$

We have two results. Inputting this into our original function gives us a general solution of:

$$x(t) = C_{1}e^{i \omega t} + C_{2}e^{-i \omega t}$$

Where $C_{1}$ and $C_{2}$ once more are arbitrary constants. But we are dealing with physical quantities that cannot take complex answers, so we need to find a way to obtain real answers. Euler's formula, obtained through Taylor polynomial expansion of the function $e^{it}$, gives us the following as a result:

$$e^{i\omega t} = \cos (\omega t) + i\sin (\omega t)$$

$$e^{-i\omega t} = \cos (\omega t) - i\sin (\omega t)$$

Replacing into our equation:

$$x(t) = C_{1}(\cos (\omega t) + i\sin (\omega t)) + C_{2}(\cos (\omega t) - i\sin (\omega t))$$

$$x(t) = (C_{1} + C_{2})\cos (\omega t) + i(C_{1} - C_{2})\sin (\omega t)$$

Making some assumptions we can say that $A=C_{1} + C_{2}$ and $B=i(C_{1}-C_{2})$. Which can then be expressed as a single cosine function through the phase shift identity.

$$A\cos(\omega t) + B\sin(\omega t) = \sqrt{A^2 + B^2} \cos (\omega t + \arctan (^B/_{A})$$[^3]

Where $\arctan (^B/_{A}) = \phi$, which is the phase change. Since $\cos (x) \leq 1$, the maximum value the function can take is $\sqrt{A^2 + B^2}$, which then corresponds to the amplitude of the wave.

This gives us our final equation:

$$x(t) = R\cos (\omega t + \phi)$$

Changing the equation through trigonometric identities to:

$$x(t)= A\cos (\omega t) \cos (\phi) - A\sin (\omega t) \sin (\phi)$$

We can relate it to our initial condition equation, where:

$$x_{0} = A\cos (\phi)$$  $$\frac{v_{0}}{\omega}= -A\sin (\phi)$$


[^1]: (Santa Cruz Institute for Particle Physics, 2009)
[^2]: (Herman, 2021)
[^3]: Through this identity, we can see how the complex part of this problem is solved.
