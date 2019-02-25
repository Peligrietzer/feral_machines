# Parasitic Disengagement

## Quick and Dirty Introduction to Evolutionary Computation

I've been thinking a lot about natural selection, lately -- not so much the
"natural" side of it, as the way it works as a general algorithm. There's a long
and enduring stream in AI research and development that falls under the general
rubric of "evolutionary computation", which implements Darwinian selection as a
generic problem-solving algorithm. In the subfield of "genetic programming", 
which is the one with which I have the most practical experience, this means
evolving populations of programs as a way of discovering means of carrying
out certain tasks. This works, comparatively, quite well when the task is
intractable in the face of less stochastic programming methods -- typically,
that is, when we're dealing with NP-hard problems.

The basic idea is just this: evolution, following an abstract but effective
Darwinian schema, only needs three things to occur: replication, variation, and
selection. It doesn't need "life". It isn't even fussy about any particular
properties of matter. Programs, in fact, are exemplary candidates for
evolution. (And you already know about memes.) It's possible -- in fact, it's
easy -- to evolve programs that are well-adapted to particular tasks, that
find optimal solutions to problems, that fuzz out leaks and holes in software,
that discover and exploit vulnerabilities, etc.

Classically, what you need to implement genetic programming is this: some way of
selecting, out of a population of (intially random) programs, candidates for
reproduction one or more "variation operators", emulating mutation or sexual
reproduction, for example, for generating new programs out of the programs
already in your population

Selection is traditionally performed with reference to the "fitness" of a
specimen, which requires you to quantify how close it comes to solving the
problem you're interested in. For classification problems, this could be tied to
accuracy, or detection rate, or whatever. For optimisation problems, it could be
tied to efficiency. Coming up with a good selection method is usually the key to
unravelling the entire problem. With that in hand, almost everything else falls
into place.

Once it's up and running, a genetic algorithm implements a form of "machine
learning", or even intelligence. There's something wonderful about this. It's
"Intelligent Design" turned on its head: instead of looking at the complexity of
life and stubbornly insist in the face of Darwinian selection that there's some
sort of divine "intelligence" behind it all, we take random, blind, natural
selection, deploy it an absolutely artificial, virtual environment and exploit
it as a form of machine intelligence! There's something sublime in this. It
thrills the fuck out of me.

![Sacculina](/img/Haeckel_Sacculina.png)

## Coevolution and Parasitism

Anyway, lately I've been studying ways of engineering co-evolution. Instead of
measuring the evolving population against some static, a priori measure of
fitness, you evolve the selection mechanism along with the population it selects
from. You evolve it, for instance, as a second population, in tension with the
first. Sometimes this is compared to the relation between host and parasite
populations, or predator and prey. The parasite poses problems to the host, and
itself has to adapt to this task. The host tries to solve these problems in
return.

There's a few ways this can go. The two populations can lock into an "arms
race", each adaptation accelerating the evolution of its opponent. It's also
possible for the two populations to collude, learning to pose as little
challenge as possible to one another, settling into a sort of oligarchal
mediocrity. An especially common outcome, however, is for the two populations to
simply disengage. This happens when the parasites and hosts lose any means of
telling the counterparts apart, when a parasite, for example, has reached such
an extreme state of virulence that every host is fails its tests in equal
measure. Imagine, for example, two populations of pong paddles, where the left
side has evolved to a point that it defeats every single right paddle with equal
(and high) probability. At this point, whatever selective pressure that the left
side imposed on the right is lost -- and vice-versa. With selection no longer
playing a role, as genetic drift comes to dominate the process. Variation
continues to occur, but it is now a purely stochastic process, a random walk.
Adaptation has stopped, and any "intelligence" that the system might have
exhibited gives way to a kind of free-floating delirium.

This is where we're at.

## Radical Postures and Memetic Drift 

It's pretty obvious that this is what's been happening in some (most) swaths of
academic philosophy (something I've stewed in, myself, for a pretty long time).
You have these entire discourses -- entire discursive populations -- that are no
longer sensitive to any selective pressures from the outside. Discourses for
whom the sciences are a sort of opaque monolithic block, and any talk about them
dismissable as "scientism", and for which politics has about as little texture
as a couple of opaque, featureless banners. What you get there is something that
I suppose you could call "memetic drift": they're not exactly stagnant --
they're actually pretty lively and volatile -- but the way they vary is almost
completely arbitrary. A random walk through academic memespace.

This seems like a pretty good way of framing political disengagement, too. I'm
not talking about apathy or listlessness here. Disengagement can be passionate.
It's even romanticised -- a self-styled "radical" posture that is so intense, so
virulent, that no adversary can measure up to it. Everything is equally
unacceptable. A sort of polarization takes place, but one that seems less and
less like an actual struggle, and certainly has less and less of an effect on
its environment (including, of course, its adversarial host).

This is a pretty abyssmal situation situation for adversarial or minoritarian
politics to find itself in. Feminism, for example, isn't currently poised to
impose any sort of unilateral hegemony from above. Until the tables turn, our
best bet is to be a clever sort of parasite, one that can steer and redirect the
evolution of the host. Politics is a craft where your best tool is your
adversary.

But we need to be virulent, too -- virulent enough, at least, to avoid falling
into the trap of collusion. There is always a risk of collusion, and if that
happens, everything that counts is extinguished. And yet impatiently ratcheting
up the virulence and shooting for a sort of holy radicalism can lead to
selective disengagement. Any chance of sculpting the adversary's political
genome is lost, along with any chance of adapting to the adversary's tactics.
All that's left is a sort of delirious drift through the ether.
