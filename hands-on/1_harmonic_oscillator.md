# The Simple Harmonic Oscillator
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

We now have what is considered a second-order differential equation. Moreover, the relationship we have is that of a function whose derivative is the same function times a constant. But we can also remember that harmonic oscillatory motion is periodic, following a sinusoidal pattern, so we can give an initial guess of our function based on sine and cosine functions. Before that, let us set some initial conditions.

At time = 0, what we will say is the following: $x(t)=x_{0}$ and $\frac{\mathrm d}{\mathrm dt}x(t)=v_{0}$. Which is saying that at time = 0, our position will be $x_{0}$, any initial position, and our velocity will be $v_{0}$, any initial velocity. 

Let's try to come up with a solution to solve our first initial condition, what we want is for our function to be $x_{0}$ or a value that maintains $x_{0}$ as itself.

When $t = 0$:

$$\cos (0) = 1$$

so maybe,

$$x(t)= x_{0}\cos (t)$$

$$x(0) = x_{0}(1) = x_{0}$$

Now let's try and solve for our second condition by taking this derivative.

$$\frac{\mathrm d}{\mathrm d t}x(t) = -x_{0}\sin (t)$$

If we were to substitute $t=0$ here, we would get 0, which is an assumption that we do not have an initial velocity. But that's a specific answer, we need a generalization.

So if we know that $\cos (0) = 1$, could we do something similar to the first case? If we want to get $v_{0}$ from our first derivative, we need to add a function that when derivated turns to cosine.

$$x(t) = x_{0}\cos (t) + v_{0}\sin (t)$$

And this still holds true for our initial conditions.

A final test would be to get the second derivative to test if it complies with $\frac{\mathrm d^2}{\mathrm d t^2}x(t) + = -\omega^2x(t)$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -x_{0}\cos (t) - v_{0}\sin (t)$$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -1(x_{0}\cos (t) + v_{0}\sin (t))$$

but $x_{0}\cos (t) + v_{0}\sin (t) = x(t)$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -1(x(t))$$

Hmm, not quite what we wanted but really close, all that we are missing is to multiply all of this by $\omega^2$ for this to hold true. This is a simple fix, we can place our constant $\omega$ in a place where it will not modify our initial conditions such as inside the trigonometric functions.

$$x(t) = x_{0}\cos (\omega t) + v_{0}\sin (\omega t)$$

But let's test it!

$$\frac{\mathrm d}{\mathrm d t}x(t) = -x_{0}\omega \sin (\omega t) + v_{0} \omega \cos (\omega t)$$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -x_{0}\omega^2 \cos (\omega t) - v_{0} \omega^2 \sin (\omega t)$$

Which does comply with our differential equation, but if we test our initial conditions, particularly velocity, we'll see it no longer holds there.

$$\frac{\mathrm d}{\mathrm d t}x(0) = -x_{0}\omega \sin (\omega (0)) + v_{0} \omega \cos (\omega (0))$$

$$\frac{\mathrm d}{\mathrm d t}x(t) = 0 + v_{0} \omega (1)$$

Thankfully this is an easy solution, by simply changing our function so that instead of just $v_{0}$, we can put $\frac{v_{0}}{\omega}$, quickly solving this issue.

$$x(t) = x_{0}\cos (\omega t) + \frac{v_{0}}{\omega}\sin (\omega t)$$

$$\frac{\mathrm d}{\mathrm d t}x(t) = -x_{0}\omega \sin (\omega t) + v_{0} \cos (\omega t)$$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -x_{0}\omega^2 \cos (\omega t) - v_{0} \omega \sin (\omega t)$$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -\omega^2(x_{0}\omega^2 \cos (\omega t) + \frac{v_{0}}{\omega} \sin (\omega t))$$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t) = -\omega^2(x(t))$$

**Harmonic Oscillator Based on Amplitude and Phase Change**

A secondary equation based on amplitude and phase change is proposed, where:

$$x_{0} = A\cos \phi$$  $$\frac{v_{0}}{\omega}= -A\sin \phi$$

Changing the equation to:

$$x(t)= A\cos \omega t \cos \phi - A\sin \omega t \sin \phi$$

Which through trigonometric identities can be simplified to:

$$x(t) = A\cos (\omega t + \phi)$$


[^1]: (Santa Cruz Institute for Particle Physics, 2009)
[^2]: (Herman, 2021)
