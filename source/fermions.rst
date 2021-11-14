Fermions and Bosons
===================

All fundamental particles can be divided into two groups: fermions and bosons.  Fermions include the quarks and
electrons that make up normal matter, as well as various more exotic particles.  Bosons are force carriers, such as the
photons that transmit the electromagnetic force and the gluons that transmit the strong force.  (I feel slightly guilty
for having just written that sentence.  You will see why in the next chapter.  But to avoid raising too many issues at
once, I will stick with the conventional description for now.)  Here are the ways in which they are conventionally said
to differ from each other.

- Fermions have half-integral spin, while bosons have integral spin.
- The wavefunction is antisymmetric under exchange of identical fermions, but symmetric under exchange of identical
  bosons.
- Fermions are bound by the Pauli exclusion principle, while bosons are not.

The first of these is a straightforward statement about their physical properties, and is easy to demonstrate
experimentally.  The other two relate as much to the mathematics we use to describe them as to the particles themselves.
Their physical significance is far less clear than is normally claimed.

Understand that when we talk about "exchanging" two identical particles, we are not referring to any physical process.
We do not mean we are actually moving any particles around.  All we are exchanging is the completely arbitrary labels
"particle 1" and "particle 2".  If the particles are truly identical, no physical property of the system can possibly
depend on our arbitrary choice of how to assign labels.  This includes, for example, the joint probability distribution.
It must be symmetric under exchange of identical particles, whether fermions or bosons:
:math:`P(\mathbf{r}_1, \mathbf{r}_2) = P(\mathbf{r}_2, \mathbf{r}_1)`.

The joint probability distribution directly corresponds to the magnitude of the wavefunction, so it too must be
symmetric.  The phase is another matter.  It is not measurable and, for all we know, may not directly correspond to any
physical property of the system.  If that is the case, it is possible it could change when we reverse the labels.

Indeed, that turns out to be true.  One can rigorously show that the wavefunction must be antisymmetric under exchange
of identical particles with half-integral spin (:math:`\Psi(\mathbf{r}_1, \mathbf{r}_2) = -\Psi(\mathbf{r}_2, \mathbf{r}_1)`),
but symmetric under exchange of identical particles with integral spin (:math:`\Psi(\mathbf{r}_1, \mathbf{r}_2) = \Psi(\mathbf{r}_2, \mathbf{r}_1)`).
This result is called the spin-statistics theorem.

Does this have any physical significance?  At first you might think not.  The overall phase of the wavefunction is
unmeasurable, so changing it cannot alter the result of any experiment.  In fact, this is a strong argument that the
wavefunction cannot directly correspond to any real, physical object.  If it did, its value could not be affected by
permuting arbitrary, physically meaningless labels.

But there is one case where it does matter.  What happens if two identical fermions are at exactly the same position,
so :math:`\mathbf{r}_1 = \mathbf{r}_2`?  In that case, we obtain :math:`\Psi(\mathbf{r}_1, \mathbf{r}_1) = -\Psi(\mathbf{r}_1, \mathbf{r}_1)`,
which is only possible if :math:`\Psi(\mathbf{r}_1, \mathbf{r}_1) = 0`.  The probability of observing two identical
fermions at exactly the same place at the same time is 0.  This is the Pauli exclusion principle.

At least, that is the conventional interpretation.  Let's take a moment to consider it more carefully.  Electrons are
charged, so they repel each other, and the strength of the repulsion goes to infinity as the distance between them goes
to zero.  We don't need a symmetry property of the wavefunction to tell us that two electrons will never be found at
exactly the same location.  We already knew that.  Most other fermions are also charged, so the same applies to them.
The exception is neutrinos, which are uncharged fermions that interact only through the weak force.  They are also
believed to repel each other, but given the very short range of the weak force, this is impossible to measure with
current technology.

In a sense, the Pauli exclusion principle tells us even less than what we already knew.  It applies only when we exchange all
relevant variables of the wavefunction, both positions and spins.  As far as it is concerned, there is no reason two
electrons cannot exist at the same position as long as they have opposite spins.  In reality, however, that can never
happen.  Electrons with opposite spin still repel each other.

Many texts confidently declare the exclusion principle has nothing to do with interactions between the particles, and
would apply even if they did not interact.  To "prove" this, they ask us to imagine two identical, non-interacting
fermions.  Of course, to the best of our knowledge, there is no such thing.  All identical fermions found in the real
world do interact.  Next they assume the wavefunction is antisymmetric under exchange of particles, and show how this
leads the particles to avoid each other.  Of course, this is a contradiction, since if they avoid each other then by
definition they do interact.

In short, they present an imaginary experiment involving particles unlike any known to exist in the real world, then
follow with two contradictory assumptions (that they do not interact, and that they do interact but in some unknown,
poorly defined way).  This is presented as somehow being a rigorous proof.

I must be careful here, because I do not want to give the impression that the Pauli exclusion principle "does not exist",
or is nothing more than Coulomb repulsion.  Dyson famously showed that atoms are much larger than would be expected
based on a simple Coulomb interaction.  Requiring the wavefunction to be antisymmetric leads to an effective "exchange
interaction" at short ranges that keeps the electrons further apart.

But the physical origin of this effect is still unknown.  What is the actual connection between the exclusion principle
and interactions between identical particles?  That is hard to say.  It certainly is noteworthy that all known fermions
repel each other.  Does this reflect some deep connection, or is it merely a coincidence?  The answer is not clear.

Piling confusion upon confusion, many sources describe the exclusion principle in a different way.  They present it as
saying two identical fermions can never have the same "quantum state" at the same time.  This is an entirely nonsensical
description, and betrays a deep misunderstanding.  A system of interacting particles has only a single "quantum state"
(that is, a single wavefunction) that describes all particles jointly, including any correlations between them.
It cannot be decomposed into separate, single-particle states.  It is meaningless to ask for the "quantum state" of a
single one of them, or to ask whether the states of two particles are the same or different.

These sources often present the following calculation, which is meant to illustrate this version of the exclusion
principle.  I must warn you before you read it that it is entirely wrong from beginning to end.  Still, it is important
to be familiar with it, since you will likely come across it.

They begin by considering two identical fermions, such as the two electrons in a helium atom, and assume the wavefunction
can be decomposed into a product of single-particle functions.

.. math::

    \Psi(\mathbf{r}_1, \mathbf{r}_2) = \Psi_1(\mathbf{r}_1) \Psi_2(\mathbf{r}_2)

Next they point out this wavefunction is not antisymmetric, and therefore is illegal for fermions.  To fix this problem,
they explicitly antisymmetrize it.

.. math::

    \Psi(\mathbf{r}_1, \mathbf{r}_2) = \Psi_1(\mathbf{r}_1) \Psi_2(\mathbf{r}_2) - \Psi_1(\mathbf{r}_2) \Psi_2(\mathbf{r}_1)

Next they ask us to suppose the two particles are in identical "quantum states", that is, that
:math:`\Psi_1(\mathbf{r}) = \Psi_2(\mathbf{r})`.  In that case, the wavefunction reduces to

.. math::

    \Psi(\mathbf{r}_1, \mathbf{r}_2) = \Psi_1(\mathbf{r}_1) \Psi_1(\mathbf{r}_2) - \Psi_1(\mathbf{r}_2) \Psi_1(\mathbf{r}_1) = 0

The problem with this calculation is simply that the true wavefunction *does not have the form given above*.
Interactions between the electrons in an atom cause them to be strongly correlated with each other.  The wavefunction
cannot in any way be written as a product of single-particle wavefunctions, with or without antisymmetrization.
Therefore it is meaningless to talk about a single electron within an atom having its own independent "quantum state".

This confusion dates back to Pauli's original formulation of the exclusion principle, which stated that two electrons in
an atom could not have the same "quantum numbers".  We cannot really fault him for this: he introduced it in 1925,
before the idea of a wavefunction had yet been developed.  It is our own fault if we keep using obsolete descriptions
long after they are replaced by more modern ones!

Now let's move on to another major source of confusion: the idea of "composite" fermions and bosons.  When multiple
fermions are strongly bound to each other, we can approximate them for many purposes as a single composite particle.
If the number of component particles is even, we say the composite particle is a boson.  If the number is odd, we say
the composite particle is a fermion.

Up to a point, this idea is not wrong.  If you combine an even number of particles that each have half-integral spin,
the total spin will be integral.  If you combine an odd number, the total spin will be half-integral.  This is
straightforward.

Likewise, each time you exchange two identical fermions, the wavefunction changes sign.  If you perform an even number
of exchanges, the result is to leave the wavefunction unchanged.  If you perform an odd number of exchanges, the
wavefunction changes sign.  This is exactly as you would expect from the above definitions.

But as you try to push the idea further, it quickly breaks down and starts to mislead you.  Consider a helium atom.  It
contains 12 quarks (two protons and two neutrons) plus two electrons.  Therefore it is a composite boson.  Bosons are
not bound by the exclusion principle and can exist at the same place at the same time.  Does this mean helium atoms can
pass through each other and exist on top of each other?  Of course not!  If you try to push two helium atoms together,
they strongly repel each other.

As another example, consider two isotopes that differ by a single neutron, such as :superscript:`12`\ C and
:superscript:`13`\ C.  One is a boson and the other is a fermion.  Therefore you would expect them to have radically
different properties.  Instead, all of their chemical interactions are identical.  Aside from experiments specifically
designed to measure mass or nuclear spin, they are nearly impossible to tell apart.

Bose-Einstein condensates are often cited as an example of atoms behaving as composite bosons.  This again is correct
up to a point.  If you cool a gas of identical atoms with integral spin to near absolute zero, they really do undergo
a transition that matches the predictions for bosons.

But it also provides a clear illustration of the limits of this description.  In their original papers on the subject,
Bose and Einstein explicitly assumed the atoms did not interact.  The theory has since been extended to account for
interactions, but only weak ones.  In practice, all experiments on Bose-Einstein condensates involve dilute gases in
which the atoms are far apart and interactions are minimized.  If they are allowed to come too close together and
interact too strongly, it is no longer valid to describe them as independent bosons.  But the ability to closely
approach each other is supposed to be one of the core features that distinguishes bosons from fermions.  The description
breaks down exactly when it is most important!  If you take it too literally, it will mislead you and produce confusion.