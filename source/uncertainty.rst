The Uncertainty Principle
=========================

Heisenberg introduced his famous uncertainty principle in 1927.  He based it on the following argument.

Suppose you want to measure the position of a particle.  You might do it, for example, by shining light on it and
detecting the reflected light.  This experiment, like all real world experiments, has limited precision.  It can only
determine the particle's position to an accuracy roughly equal to the wavelength of the light.

The interaction between the particle and the light perturbs the motion of the particle, imparting some momentum to it.
We do not know the exact change in momentum (that would require knowing precise details of the interaction that cannot
be determined from the experiment), but we do know its magnitude must be on the order of the amount of momentum carried
by the light.  That is inversely proportional to its wavelength.  Combining these two results, Heisenberg obtained the
following very approximate inequality.

.. math::

  \Delta x \Delta p \gtrsim 2 \pi \hbar

where :math:`\Delta x` is the uncertainty in our measurement of the position and :math:`\Delta p` is the uncertainty in
the momentum after completing the measurement.  We could reduce :math:`\Delta x` by using light with a shorter
wavelength, but then we would disturb the particle more and increase the uncertainty in its momentum.  Alternatively we
could decrease :math:`\Delta p` by using light with a longer wavelength, but then we would be able to measure the
position less precisely.

This is a purely mechanistic argument based on the practical details of performing measurements.  It also requires only
classical physics.  Nothing about it is specific to quantum mechanics.

The uncertainty principle was later reinterpreted as a statement about the quantum mechanical wavefunction.  If a
particle's position is precisely known, its wavefunction is a delta function in position space.  This corresponds to a
plane wave in momentum space, meaning the momentum is completely unknown.  Likewise, if the momentum is precisely known,
the wavefunction is a delta function in momentum space and a plane wave in position space.  If we want to know both
position and momentum at the same time, we must choose a wavefunction that is localized but not precisely defined in
both spaces.  The best we can do turns out to be a Gaussian distribution, whose Fourier transform is also a Gaussian.
This leads to the inequality

.. math::

  \Delta x \Delta p \gt \hbar / 2

where :math:`\Delta x` and :math:`\Delta p` are now more precisely defined as being the standard deviations of the
position space and momentum space representations of the wavefunction.

These two "uncertainty principles" seem entirely different from each other.  They are based on entirely different
arguments and relate to different phenomena (the practical limitations of the measurement process versus the intrinsic
properties of the wavefunction).  Yet they reach the same conclusion to within a small constant factor.  Is this just a
remarkable coincidence, or does it reflect a deeper connection?

If we view the wavefunction as a description of our knowledge about a system, the agreement is not surprising.  It is
only natural we would have settled on a description that reflects the actual limits of what we can know.  On the other
hand, if we interpret the wavefunction as a physical object rather than a mathematical abstraction invented by humans,
the agreement is harder to explain.  How does a purely classical description of the measurement process produce the
correct result for an inherently non-classical phenomenon?

Although the two arguments lead to the same result, there is a critical difference between them.  Heisenberg's
mechanistic argument applies only to initial value problems, not to boundary value problems.  We can see this from a
simple example.

Consider a single particle moving in free space.  We first measure its position by reflecting light off it.  Then we
wait for a time interval :math:`t`, measure its position a second time, and find it has traveled a distance :math:`x`.
We can conclude that between the two measurements, it must have been moving with velocity :math:`x/t`.

Of course, there is uncertainty in all of these values.  The distance travelled is only measured to within some
uncertainty :math:`\Delta x` determined by the wavelength of the light.  The time interval between the measurements can
only be controlled to some precision :math:`\Delta t`.  The ratio of distance to time therefore is also uncertain.

But we are not bound by the uncertainty principle.  We can make :math:`\Delta x` arbitrarily small by using shorter
wavelength light.  This does not increase the uncertainty in the velocity, because :math:`x/t` is a direct measure of
how quickly the particle was moving *between* the two measurements, after its momentum was disturbed by the first
measurement and before it was disturbed by the second measurement.  We also can make the uncertainty in the velocity
smaller by increasing :math:`t`.  Simply by choosing the wavelength of light and the time interval between the
measurements, we can simultaneously know both position and momentum to arbitrary precision at every intermediate time
between the two measurements.

Having determined the momentum through our two measurements, we might be tempted to extrapolate to earlier and later
times.  At this point we run into the uncertainty principle again.  Each of the measurements alters the momentum in an
unknown way.  We know the momentum before the first measurement is different from :math:`x/t`, and after the second
measurement it is different again, but we do not know the exact values.  The more precisely we perform the position
measurements, the more uncertain the momentum becomes.

If we instead view the wavefunction as a physical object rather than a mathematical abstraction, we are forced into a
much more convoluted interpretation.  Although we measured the particle to have traveled a distance :math:`x` in time
:math:`t`, we are not allowed to conclude it was traveling with velocity :math:`x/t`!  In this view, the first position
measurement leads to a wavefunction that is localized in position and therefore uncertain in momentum.  From that point,
the uncertainty in position grows steadily.  By the time we perform the second measurement, the wavefunction has come to
be widely distributed.  We measure the distance traveled to be :math:`x`, but we could just as easily have gotten a
different result.  Until we perform the second measurement and collapse the wavefunction, the particle's position is
highly uncertain.  The particular position it happens to collapse to implies nothing about its momentum prior to the
measurement.

In the same paper introducing the position-momentum uncertainty principle, Heisenberg also proposed a second uncertainty
principle involving energy and time.  He based it on a mechanistic argument similar to the other one.  He considered a
typical experiment used to measure energy and argued that the less time one spent performing the measurement, the less
accurately one could determine the result.  A simple argument led to the approximate inequality

.. math::

  \Delta E \Delta t \gtrsim 2 \pi \hbar

where :math:`\Delta E` is the uncertainty in the measured energy of a system and :math:`\Delta t` is the amount of time
taken to measure it.  

This result is fundamentally different from the position-momentum uncertainty principle.  "The time taken to perform a
measurement" is not itself a measurable quantity.  It is not something you can calculate from a wavefunction.  It is a
property of how you perform an experiment.

Just as the position-momentum uncertainty principle was later reinterpreted, the energy-time principle was also
reinterpreted, but this time the meaning changed enormously in the process.  Consider an eigenstate of the Hamiltonian.
This is a state with precisely defined energy.  Because it is an eigenstate, all measurable quantities are independent
of time.  They never change.

Now consider a superposition of states with similar but slightly different energies.  This is not an eigenstate of the
Hamiltonian, so measurable quantities do change with time.  The wider the spread in energies, the more quickly they
change.  One can derive the inequality

.. math::

  \Delta E \Delta t \gt \hbar / 2

where :math:`\Delta E` now refers to the spread in energy of the states making up the superposition, and :math:`\Delta t`
describes the time scale over which any measurable quantity *other than energy* changes.

Beware of a common misunderstanding about the energy-time uncertainty principle.  Many authors claim it means you can
violate conservation of energy by an amount :math:`\Delta E`, as long as you only do it for a short time
:math:`\Delta t`.  This claim is entirely wrong!  The expectation value of the Hamiltonian
:math:`\left\langle \Psi | H | \Psi \right\rangle` is conserved by the Schrödinger equation.  That is what conservation
of energy means in quantum mechanics.  It is an exact law.  It cannot be violated by even the smallest amount, no matter
how short a time you do it for!