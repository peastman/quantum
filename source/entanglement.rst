Entanglement, Hidden Variables, and Bell's Inequality
=====================================================

Entanglement is often presented as a mysterious phenomenon, but it is actually a very simple concept.  When we say two
particles or two degrees of freedom are entangled, that simply means they are correlated with each other.  The
wavefunction, and therefore the joint probability distribution, cannot be factored into a product of single-particle
functions.  Measuring a property of one particle provides information about the probability distribution of the other
particle.

Consider one of the classic examples used to demonstrate entanglement.  An atom with zero angular momentum emits two
electrons in different directions.  Conservation of angular momentum requires the two electrons to have opposite spin
along any axis.  If you measure the spin of one electron, you immediately know what the spin of the other one must be
even though you have not yet measured it.  That is the essence of entanglement.

So far we have no reason to think anything mysterious is going on.  The two electrons originated from the same atom, so
of course we expect them to be correlated.  A hidden variable theory would say that both electrons had well defined spin
before you measured either one.  The measurement just provided new information.

But that is not how quantum mechanics conventionally describes it.  The standard description is to say the electrons are
in a superposition of states: :math:`\left| \uparrow \downarrow \right\rangle + \left| \downarrow \uparrow \right\rangle`.
It is certain that the particles have opposite spin, but which is up and which is down does not become defined until you
perform a measurement of one.  At that point the wavefunction collapses and the spins of both particles become fully
defined.  A measurement on one particle is supposed to somehow change the state of the other particle.  This is the idea
that Einstein famously ridiculed as "spooky action at a distance."

Is this a real physical difference, or only a semantic one?  Are these just two equivalent ways of describing the same
thing, or can one experimentally distinguish between them?

In 1964, John Bell proposed a variation on this experiment. [#f1]_  In his version, each of the two measuring devices can be
configured to measure spin along multiple axes.  The experiment is repeated many times, each time randomly selecting one
of the possible axes for each device.  Under an assumption he considered to be reasonable for most hidden variable
theories, he showed the results must satisfy a particular inequality.  On the other hand, the predictions of quantum
mechanics do not satisfy that inequality.  Since that time, many experiments have been performed to try to test Bell's
inequality, and many of them are claimed to have observed violations of it, thus (supposedly) disproving the possibility
of hidden variable theories.

(In addition to the inequality originally derived by Bell, a number of other similar inequalities have since been
derived.  They are collectively known as "Bell-type inequalities".  For simplicity I will keep talking about "Bell's
inequality", but understand that when I say this I am really talking about the whole class of inequalities.)

Let's take this from the beginning and try to understand what is actually the case.  To start with, what
assumptions is Bell's inequality derived from?  Even this simple question is already the source of much confusion.  You
can find many sources giving conflicting answers to it.  In fact, it is derived from only a single assumption: that the
result measured by each device is statistically independent of which axis the *other* device is set to measure.  More
formally, we assume the conditional probability distribution factorizes:

.. math::

    P(A,B|S_A,S_B,\lambda) = P(A|S_A,\lambda) P(B|S_B,\lambda)

where :math:`A` and :math:`B` are the results measured by the two devices, :math:`S_A` and :math:`S_B` are the settings
of the two devices (that is, which axis each one is configured to measure), and :math:`\lambda` represents the values of
all hidden variables in the system.

Take a moment to consider this assumption.  We are not assuming the *results* are independent.  After all, they are
measurements of two particles that originated from the same atom, so we expect them to be correlated with each other.
We also do not assume a device's result will be independent of its *own* setting.  Of course we expect its setting to
influence what result it produces.  But we assume the result measured by the first device should be independent of how
the second device is configured.

This assumption certainly seems plausible, but it also is not obvious that it must be true.  We can easily imagine
mechanisms that might lead to correlations between the measuring devices.  Ideally we would derive this assumption from
other, more clearly justified assumptions.  But no rigorous derivation is available.  We simply must accept it as a
postulate.

Lacking a rigorous derivation, most people try to justify it by approaching the question from the opposite direction.  They
assume the results must be uncorrelated *unless some mechanism causes them to become correlated*.  Then they enumerate
every mechanism they can think of, assume each one does not exist, and take that as a justification.  This approach can
be useful for developing intuition, but do not mistake it for a rigorous derivation.  For example, it is impossible to
be certain there is no other mechanism you simply have not thought of!

Nonetheless, let's try following this approach.  What mechanisms could create correlations, such that the equation above
would not hold?

One possibility is that the two particles (or alternatively, the two detectors) are directly linked in some way, such
that when you measure one particle, the other is instantly affected as well.  This idea is called "non-locality".  It
means an event at one point in space directly affects some other point, without the influence needing to propagate
through the intervening space.  In the conventional view of quantum mechanics, the collapse of the wavefunction is
non-local.  When you measure one particle the wavefunction collapses, instantly affecting the other particle no matter
how far apart they are.

Some hidden variable theories are also non-local, and therefore not bound by Bell's inequality.  For example, in pilot
wave theory, the particles obey Newtonian dynamics (a local theory), while the pilot wave follows the same rules as the
wavefunction in quantum mechanics (a non-local theory).

The idea of non-locality is controversial.  Aside from the collapse of the wavefunction, all known physical laws satisfy
locality.  Does this reflect some deep truth about the nature of the universe?  If so, then we must dismiss any
non-local theory.  But this is not a rigorous argument.  There are theoretical reasons to suspect non-locality might be
possible.  For example, the holographic principle hypothesizes that our familiar four dimensional spacetime is an
emergent phenomenon, and the true degrees of freedom making up the universe exist on some lower dimensional surface.
Each point in spacetime would then be created by the interaction of many degrees of freedom, and each degree of freedom
would influence many points in spacetime.  That suggests non-local effects could be possible.

Of course, this is pure speculation.  We should not dismiss the possibility of non-locality, but we also cannot assume
it exists.  We should demand very powerful evidence to support any claim of non-locality.

Perhaps we are taking the rules of quantum mechanics too literally.  We conventionally describe wavefunction collapse as
an instantaneous process, but that may not really be true.  We now understand that it involves the creation of
decoherence as the system and environment interact with each other.  That is a gradual, continuous process.  If we
accept that wavefunction collapse takes a finite time and involves interactions propagating through space in the normal
manner, there is no longer anything non-local about it.

Some hidden variable theories make that explicit.  For example, Stochastic Electrodynamics derives entanglement as a
consequence of the particles interacting through the electromagnetic field.  It is a local theory, yet it still predicts
that Bell's inequality may be violated.

In principle we should be able to test this experimentally.  In a local theory, no influence can propagate faster than
the speed of light.  (Strictly speaking, that is a separate assumption.  One could imagine a theory that forbids
instantaneous, non-local influences while still allowing ones that propagate faster than light.  But in practice, nearly
all local hidden variable theories do make this assumption.)  We could let the two particles travel a very long distance
from each other, then perform the measurements very quickly, so we get the results before any signal could possibly
travel from one to the other.

When working with electrons or other massive particles, this turns out to be very difficult.  Massive particles
necessarily travel slower than light, usually much slower.  It also is hard to transport them over long distances while
isolating them from any interactions that would destroy the entanglement.  As a rule, tests of Bell's inequality on
massive particles tend to involve short distances and long time scales.  They can observe violations of the inequality,
but they cannot determine whether the mechanism responsible is a local or non-local one.

Many experiments have tried to work around this by using light in place of massive particles.  It has the two advantages
of moving much faster, and being much less susceptible to unwanted interactions.  In experiments with light,
entanglement has been demonstrated over distances of many kilometers.  Many of the people conducting these experiments
also claim to have observed violations of Bell's inequality.  Nearly all of these claims are false.  In fact, they never
had the slightest possibility of observing a violation.

To understand this, we need to distinguish between the idealized experiments we imagine doing and the real experiments
that are done in practice.  In the ideal experiment Bell proposed, two particles enter two measuring devices.  Each one
reports whether the particle's spin was up or down.  In a real experiment there is a third possibility: the device may
simply fail to detect the particle and not report anything at all.  This difference turns out to be critically
important.  The more particles that are missed, the harder it is for Bell's inequality to be violated.  In fact, if more
than one third of the particles are missed, it is mathematically impossible for the inequality to be violated.  Any
experiment in which the measuring devices have detection efficiencies less than 67% has no possibility of ever observing
a violation.

The very best photodetectors have detection efficiencies of only around 30%, far too low to be capable of testing Bell's
inequality.  How, then, do experimenters claim to have observed violations despite the clear impossibility of doing so?

The answer is that they make an extra assumption, the so-called "fair sampling assumption".  It states that the hidden
variables of the particles that were missed followed exactly the same distribution as those of the particles that were
detected.  No justification is given for this assumption.  Let's take a moment to consider whether it is reasonable or
not.

A stream of particles enters a detector.  Their hidden variables follow some distribution.  They are divided into two
groups, those which get detected and those which do not.  The fair sampling assumption states that both groups still
have exactly the same distribution of hidden variables.  In other words, the hidden variables must be completely
independent of whether a particle gets detected.  *If* it is detected, the hidden variables are allowed to influence
what result the detector reports, but they cannot influence in any way whether it gets detected or not.

Of course this is absurd.  For a deterministic hidden variable theory, in fact, the hidden variables are quite literally
the only factor that can possibly determine why some particles are detected and others are not.  Yet people frequently
choose to assume otherwise.  Worse, they often try to pass off the fair sampling assumption as routine, a minor
technical detail (often referring to it as a "loophole"), when in fact it is directly contradicted by essentially all
the hidden variable theories they claim to be testing.

There is another mechanism that could potentially account for violations of Bell's inequality.  It is one that Bell
himself did not consider, and in fact was generally ignored for some years, simply because no one had thought of it.
When we measure the spin of a particle we alter its properties and force it to align with the detector.  Perhaps the
influence of that measurement propagates backward, forcing it to have a particular spin before it enters the detector.
The influence extends all the way back to when the two particles were first emitted, and thus can affect the other
particle as well.

The idea of effects propagating backward in time is called "retrocausality".  It is a somewhat boggling idea when you
first encounter it, but it is not nearly so speculative as you might think.  On the contrary, all the fundamental laws
of physics appear to treat both directions in time identically.  More precisely, all available evidence indicates that
CPT (Charge-Parity-Time) invariance is an exact symmetry of the universe.  If you exchange what we call "forward" and
"backward" in time, while also exchanging the labels "left" and "right" and the labels "positive charge" and "negative
charge", all fundamental laws are left unchanged.  There appear to be two completely equivalent ways of describing the
universe.  As far as the fundamental laws are concerned, it is entirely arbitrary which one you choose.  Yet the
direction called "forward in time" by one description is called "backward in time" by the other one.

Of course, this conflicts with our intuitive view that time is asymmetric, that it only "moves" in one direction.  That
asymmetry is now understood to be entropic in nature, however.  We refer to the direction of increasing entropy as
"forward in time".  In our local region of spacetime, that means the direction pointing away from the big bang.  It is
a property of how matter and energy are distributed in our neighborhood, not of any fundamental property of time.

A number of hidden variable theories have been proposed that make use of retrocausality.  These theories emphasize that
all physics problems must be viewed as boundary value problems, not as initial value problems.  A single measurement of
a system is insufficient to determine its behavior at other times.  But if you make two measurements at two different
times, you can uniquely determine its state at every intermediate time between the two measurements.

To understand retrocausality, you must let go of the presentist mindset ("only the present moment exists") and accept
a universalist one (all times exist on an equal footing).  If you think of a measurement "altering" a particle, and
the effect of that alteration "propagating backward", you will become confused.  It is too different from our intuition.
But if you think of a measurement as just setting a boundary condition that must be obeyed by a partial differential
equation, much of the confusion disappears.  If you pull on either end of a string, the tension at every point in the
string increases.  There is no inherent order to them.  You cannot say that the string "begins" at one end and "ends" at
the other.  Both ends exist on an equal footing.

When someone denies the possibility of retrocausality, they are asserting that the laws of nature distinguish between
the two possible descriptions allowed by CPT invariance.  That they are not really equivalent, and only one of them is
"right".  We have no evidence at all to support that claim.  We therefore must accept retrocausality as entirely
plausible, perhaps even likely.

It is hard to explain why so many people are ready to embrace a non-local theory yet strongly resist a retrocausal one,
even though the latter is so much better justified by evidence.  I suspect this is mainly just a matter of familiarity.
In introductory classes, quantum mechanics is usually presented as being non-local, and retrocausality is rarely
mentioned.  Having been taught this, we accept it as "what everyone knows" and resist any challenge to it.

There is yet another mechanism that could account for violations of Bell's inequality.  Perhaps the spin of the first
particle and the setting of the second detector are correlated, not because either one influences the other, but because
some third factor influences both of them.  Perhaps some initial condition of the environment influences how the
particle gets emitted, and also influences how the detector's setting gets chosen, in such a way that they become
correlated with each other.  This is called "superdeterminism".

It is hard to imagine what kind of mechanism could produce correlations of this sort.  I am not aware of any concrete
theory that uses superdeterminism to explain entanglement.  On the other hand, just because we cannot think of a
mechanism, that does not prove no such mechanism is possible.  This is another assumption we need to make.

There is yet another possibility we must consider.  Perhaps the results of the experiment are correlated, not because of
any physical mechanism, but because spurious correlations are artificially introduced by the experimental protocol and
data analysis.  This possibility has recently begun to receive increasing attention.  To understand it, we must again
distinguish between the idealized experiments we imagine doing and the real experiments we can actually perform.

In the idealized experiment proposed by Bell, pairs of entangled particles are generated and directed toward two
measuring devices.  The devices determine the spins of their respective particles.  The resulting data is a list of
particle pairs, along with the measured spin for each particle in a pair.

Real experiments are very different.  A source emits particle pairs at unknown, unpredictable times.  The interval
between emission events can be extremely variable, including the possibility of two pairs sometimes being produced in
rapid succession.  Each measuring device detects a different subset of the particles directed toward it.  After a
detection event, the device has a dead time during which it is unable to register any further events.  The devices are
subject to noise, and therefore will occasionally produce a false detection when no particle was actually present.  The
probability of a false detection may vary depending on the time since the last detection.

The upshot of this is that each detector produces a seemingly random sequence of events, and there may be little obvious
connection between the events from the two detectors.  The experimenter must somehow attempt to match them up to produce
pairs of events that are assumed to represent entangled particles.  Often this is done in a very primitive way: simply
dividing the data into fixed time windows and noting whether each detector did or did not produce a detection during
each window.

Authors have recently shown how this process can introduce spurious correlations that were not present in the raw data
and that violate Bell's inequality.  In fact, it has been experimentally demonstrated that when the two detectors
receive particles from completely independent, uncorrelated sources, the standard analysis concludes that Bell's
inequality is strongly violated. [#f2]_  Of course, this has nothing to do with entanglement.  It is simply measuring the
probability of two detections randomly occurring close together.

To their credit, experimenters have worked hard to try to address these problems, and they have made good progress on some of
them.  Unfortunately, the hype tends to run far ahead of the reality.  Each new experiment is typically proclaimed to be
a "loophole-free test of Bell's inequality", even though it has not addressed all of the issues described above.  The
interpretations loaded onto these experiments run even farther ahead of anything justified by experiment.  For example,
numerous authors have declared that these experiments have "disproved local realism", without ever considering
retrocausality as an alternative explanation.

And of course, it is critical to remember that this whole approach of trying to enumerate mechanisms is not
mathematically rigorous.  At best it is a way of trying to build intuition, and intuition can be misleading.  The only
truly rigorous derivation of Bell's inequality begins from an assumption about probability distributions.  If we are not
willing to accept that assumption as self-evident on its own merits, then all our conclusions must be viewed as
provisional.  It cannot be derived from anything else.  No amount of clever experimental design can change that.  Even
the question of whether it is possible to write a probability distribution, or how to define what that probability
distribution means, turns out to involve a series of subtle, hard to justify assumptions.  I will touch on a few of
these issues in the next chapter.

----

.. [#f1] J.S. Bell.  "On The Einstein Podolsky Rosen Paradox."  Physics 1(3): 195-200 (1964).
.. [#f2] M. Iannuzzi, R. Francini, R. Messi, D. Moricciani.  "Bell-type polarization experiment with pairs of
         uncorrelated optical photons."  Physics Letters A 384(9): 126200 (2020).