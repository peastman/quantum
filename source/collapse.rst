The Collapse of the Wavefunction
================================

Many sources include an additional postulate that I have omitted.

.. admonition:: Postulate 5

    When you perform a measurement of the quantity corresponding to an operator :math:`\Omega` and obtain the eigenvalue
    :math:`\omega` as a result, immediately after the measurement the wavefunction is given by
    :math:`\left| \Psi \right\rangle = \left| \omega \right\rangle`, where :math:`\left| \omega \right\rangle` is the
    corresponding eigenvector.

The wavefunction is said to "collapse" from a superposition of many eigenstates down to a single eigenstate.  Originally
this postulate was believed to be necessary to reproduce experiment, and many sources still include it.  It was (and
continues to be) the source of much confusion, such as the idea of a "quantum leap" in which a particle was imagined to
jump discontinuously from one position to another without ever passing through the space in between.

We now understand this postulate is not needed.  We can explain the relevant experiments using only the other
postulates.  The inventors of quantum mechanics thought they needed it because they did not include a proper description
of the measuring device in their theory.  They insisted on treating the measuring device classically, using quantum
mechanics only for the system being measured.  When you unify them, treating the measuring device and measured object as
parts of a single combined system that follows a single set of rules, the phenomenon traditionally described as
"collapse" appears naturally.

We can see this with a simple example.  Suppose an operator has two eigenvectors :math:`\left| A \right\rangle` and
:math:`\left| B \right\rangle`.  Suppose the wavefunction is initially a superposition of the two.

.. math::

    \left| \Psi \right\rangle = c_a \left| A \right\rangle + c_b \left| B \right\rangle

By applying the Born rule, we can compute the probability that a measurement will yield either :math:`a` or :math:`b`.
Recall that :math:`\left| A \right\rangle` and :math:`\left| B \right\rangle` are eigenvectors of the same operator.
This requires them to be orthonormal, so :math:`\left\langle A | A \right\rangle = \left\langle B | B \right\rangle = 1`
and :math:`\left\langle A | B \right\rangle = 0`.

.. math::

    P(a) &= | \left\langle A | \Psi \right\rangle |^2 \\
         &= | c_a \left\langle A | A \right\rangle + c_b \left\langle A | B \right\rangle |^2 \\
         &= | c_a \cdot 1 + c_b \cdot 0 |^2 \\
         &= | c_a |^2

and similarly

.. math::

    P(b) &= | c_a \left\langle B | A \right\rangle + c_b \left\langle B | B \right\rangle |^2 \\
         &= | c_b |^2

This is the traditional approach, in which we describe only the system being measured and ignore everything outside it.
Now let's expand the state space to include both.  Let :math:`\left| E \right\rangle` represent the state of the
environment, which includes everything that will be influenced by the measurement: the measuring device, any recording
device the result will be written to, even a person who will look at the result.  The state of the extended system is
:math:`\left| \Psi \right\rangle \otimes \left| E \right\rangle`.

Now we perform a measurement.  What does that mean?  Simply that we allow the measuring device and measured object to
interact with each other.  The measuring device is modified by the interaction, such that we can later look at the
measuring device and, based on its state, learn something about the object it measured.  In other words, the state of
the environment becomes correlated with the state of the object.  The combined wavefunction is now

.. math::

    \left| \Psi \right\rangle = c_a \left| A \right\rangle \otimes \left| E_a \right\rangle + c_b \left| B \right\rangle \otimes \left| E_b \right\rangle

Next we can perform a second measurement.  We will again determine the state of the object, but we will also look at the
device used in the first measurement to learn what its result was.  This will tell us whether the two measurements
produced the same result or different results.

This time we will just use the Born rule.  The probability that both measurements produced :math:`a` is

.. math::

    P(a, E_a) &= | c_a \left\langle A | A \right\rangle \left\langle E_a | E_a \right\rangle + c_b \left\langle A | B \right\rangle \left\langle E_a | E_b \right\rangle |^2 \\
              &= | c_a |^2

and similarly

.. math::

    P(b, E_b) = | c_b |^2

But now we can also look at cross terms.  What is the probability that the first measurement produced :math:`a` and the
second one produced :math:`b`?

.. math::

    P(b, E_a) &= | c_a \left\langle B | A \right\rangle \left\langle E_a | E_a \right\rangle + c_b \left\langle B | B \right\rangle \left\langle E_a | E_b \right\rangle |^2 \\
              &= | c_b \left\langle E_a | E_b \right\rangle |^2

What does :math:`\left\langle E_a | E_b \right\rangle` equal?  We have not explicitly assumed :math:`\left| E_a \right\rangle`
and :math:`\left| E_b \right\rangle` are orthogonal to each other, but in practice they clearly must be, or close enough
that they might as well be.  In order to perform a measurement, the environment needs to change in a macroscopic way
based on the thing being measured.  Otherwise, we could not use it to reliably determine what result was measured.
Ultimately we are talking about the difference between the message "State A" appearing on a computer screen and "State B"
appearing on the same screen.  These have negligible overlap with each other.  To very high accuracy,
:math:`\left\langle E_a | E_b \right\rangle = 0` and therefore :math:`P(b, E_a) = 0`.

Therefore, if you perform two measurements of the same quantity immediately after each other, they will always produce
the same result.  The chance of getting different results is negligible.  This is what we mean by "the collapse of the
wavefunction".

Notice that we did not assume anything about how the object being measured is affected by its interaction with the
measuring device.  You might think you could prevent its wavefunction from collapsing by performing the measurement very
carefully, so as to affect it as little as possible.  In fact, that would make no difference at all.  Instead, you would need to
minimize the effect on the measuring device, but if the measuring device were not affected, that would mean you had not
measured anything.

This calculation is simple, easy to follow, and frustratingly unenlightening.  It leaves us just as mystified as ever
about the mechanism responsible for wavefunction collapse.  That is because we used the Born rule, but we are still
viewing the Born rule as nothing more than an empirical observation.  We have no idea why it happens to work.  If we
want to understand the mechanism behind wavefunction collapse, we need a deeper theory that can explain the mechanism
behind the Born rule.  I will discuss some possibilities for that deeper theory in later chapters.

In discussions of this subject, you will sometimes come across the term "decoherence".  This is a more general framework
for the calculation presented above.  Initially, the system being measured is said to be in a "coherent" state.  It is a
sum of basis functions that can interfere with each other, leading to quantum interference effects.  As it interacts
with the environment, each basis function becomes correlated with the environment in a different way.
:math:`\left| A \right\rangle \otimes \left| E \right\rangle` turns into :math:`\left| A \right\rangle \otimes \left| E_a \right\rangle`.
Interference disappears, because each basis function is now associated with a macroscopically different state of the
environment.  The state is no longer coherent.

People sometimes claim that decoherence "explains" the collapse of the wavefunction.  That is incorrect.  Decoherence
simply refers to the appearance of correlations between the system being measured and its environment as they interact.
To get from those correlations to the wavefunction collapsing, we must invoke the Born rule.  A full explanation of
collapse must therefore include an explanation of the Born rule.