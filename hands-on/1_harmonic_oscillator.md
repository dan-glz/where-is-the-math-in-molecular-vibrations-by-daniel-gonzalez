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

At time = 0, what we will say is the following: $x(t)=x_{0}$ and $\frac{\mathrm d}{\mathrm dt}x(t)=v_{0}$. Which is saying that at time = 0, our position will be $x_{0}$, any initial position, and our velocity will be $v_{0}$, any initial velocity. Let us say our initial guess is the following:

$$x(t)=x_{0}\cos \omega t + b\sin \omega t$$

We can try and prove this by making sure our initial conditions are met.

$$x(0)=x_{0}\cos \omega (0) + b\sin \omega (0)$$

$$x(0)=x_{0}\cos (0) + 0 = x_{0}$$

And to prove our second condition:

$$\frac{\mathrm d}{\mathrm d t}x(t) = -\omega x_{0} \sin \omega t + \omega b \cos \omega t$$

$$\frac{\mathrm d}{\mathrm d t}x(0) =  \omega b $$

From this we can deduce that $v_{0}=\omega b$ and so $b=\frac{v_{0}}{\omega}$.

So our function has been solved for our unknown and works for our initial conditions, but now needs to be tested if it works as a solution to our first equation: $\frac{\mathrm d^2}{\mathrm d t^2}x = -\omega^2x$.

$$x(t)=x_{0}\cos \omega t + \frac{v_{0}}{\omega}\sin \omega t$$

$$\frac{\mathrm d}{\mathrm d t}x(t)=-\omega x_{0} \sin \omega t + v_{0} \cos \omega t$$

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t)=-\omega^2 x_{0} \cos \omega t - \omega v_{0} \sin \omega t$$

But we can factor out $-\omega^2$.

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t)=-\omega^2 (x_{0} \cos \omega t + \frac{v_{0}}{\omega} \sin \omega t)$$

Which is nothing more than:

$$\frac{\mathrm d^2}{\mathrm d t^2}x(t)=-\omega^2 x(t)$$

**Harmonic Oscillator Based on Amplitude and Phase Change**

A secondary equation based on amplitude and phase change is proposed, where:

$$x_{0} = A\cos \phi$$  $$\frac{v_{0}}{\omega}= -A\sin \phi$$

Changing the equation to:

$$x(t)= A\cos \omega t \cos \phi - A\sin \omega t \sin \phi$$

Which through trigonometric identities can be simplified to:

$$x(t) = A\cos (\omega t + \phi)$$


[^1]: (Santa Cruz Institute for Particle Physics, 2009)
[^2]: (Herman, 2021)
