The Postulates of Quantum Mechanics
===================================

In this chapter I will review the postulates of quantum mechanics as they appear in the familiar Schrödinger
formulation.  The exact way they are stated varies between sources.  Some sources include one or two postulates that
are not strictly necessary and can be derived from the others.  The following is a fairly typical version.

.. admonition:: Postulate 1

    The state of an isolated physical system at a single point in time is described by a complex valued wavefunction
    :math:`\Psi(\mathbf{r}_1, \mathbf{r}_2, ...)`, where :math:`\mathbf{r}_1`, :math:`\mathbf{r}_2`, etc. are the
    positions of the particles that make up the system.

.. admonition:: Postulate 2

    For every measurable quantity, there is a Hermitian operator that acts on the space of wavefunctions.

There is no physics in these two postulates.  They just establish a mathematical vocabulary.  Taken on their own, they
mean nothing and predict nothing.  So if you have trouble understanding what it means for a Hermitian operator to
represent a measurable quantity like position or momentum, that is because there is nothing to understand!  The physics
comes in the next two postulates.

.. admonition:: Postulate 3 (the Schrödinger equation)

    The wavefunction evolves with time according to the Schrödinger equation:
    
    .. math::

        i \hbar \frac{d \Psi}{dt} = H \Psi

    where :math:`H` is the Hamiltonian operator.

Strictly speaking this is incorrect, since the Schrödinger equation is not Lorentz invariant.  When relativity is
important, we must instead use the Dirac equation or the Klein-Gordon equation.  For many purposes, the non-relativistic
version is sufficient.

The final postulate, known as the Born rule, describes what happens when we perform measurements.  It is the source of
much of the confusion that surrounds quantum mechanics.

.. admonition:: Postulate 4 (the Born rule)

    When you perform a measurement of the quantity corresponding to an operator :math:`\Omega`, the result will always
    be one of the eigenvalues of the operator.  The probability of measuring a particular eigenvalue :math:`\omega` is
    equal to :math:`| \left\langle \omega | \Psi \right\rangle |^2` where :math:`\left| \omega \right\rangle` is the
    corresponding eigenvector and :math:`\left| \Psi \right\rangle` is the current value of the wavefunction.

Let's start with the first postulate.  What does it mean to describe the state of a system with a wavefunction?  It is very
confusing when we first meet it, because it is so different from what we are used to.  In classical mechanics, the state
of a system is fully specified by the position and momentum of each particle it contains.  For :math:`N` particles in
three dimensions, it is specified by :math:`6N` numbers.  In contrast, the wavefunction is specified by two numbers
(because it is complex) for *every point in a* :math:`3N` *dimensional space*.  That is a vastly larger amount of
information.  In fact, if we do not discretize the particle positions, it is infinite.

Perhaps it is only confusing because we are comparing apples to oranges.  Classical mechanics is usually applied to
macroscopic objects whose positions and momenta can be measured to high accuracy.  In that case, it makes sense to treat
them as precisely, simultaneously knowable.  Quantum mechanics is usually applied to atoms and electrons which we cannot
precisely measure or control.  We have no device that can determine the exact position of every electron in an
atom.  Since we cannot know them, it makes more sense to talk about their joint probability distribution
:math:`P(\mathbf{r}_1, \mathbf{r}_2, ...)`.  If we want to predict the distribution's time evolution, we also need the
derivative :math:`dP/dt`.  Together they contain two numbers for every point in a :math:`3N` dimensional space, exactly
the same as the wavefunction.

Is the wavefunction nothing more than a trick for bundling a joint probability distribution and its time derivative into
a single object?  We do not know, but it is entirely possible.

Notice that the postulates make no mention of spin.  In this, I am following convention.  Usually they are first stated
without spin, and then it is awkwardly bolted on later.  When using the Dirac equation to incorporate relativity, spin
emerges in a much more natural way.  Do not think that means it "explains" spin, however.  It seems likely that spin is
in some way related to relativity, but it is still a mysterious property whose nature is not understood.  For the
moment, I will just acknowledge that we must include spin if we want to correctly predict experiments, and leave it at
that.

Now let's consider the Born rule.  It is a simple rule, but also seems completely arbitrary.  Why should measurements
happen to follow this particular rule?  For that matter, what does it even mean to "perform a measurement"?  These
questions have been debated endlessly for the last century.  I will have much more to say about them in later chapters,
but for the moment let me just repeat what I said before: quantum mechanics is nothing more than a set of rules for
predicting experiments.  They have no justification beyond the fact that they work.  If we want more, we will need to
look for a deeper theory.