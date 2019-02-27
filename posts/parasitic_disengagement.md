# Parasitic Disengagement and Memetic Drift

## Quick and Dirty Intro to Evolutionary Computation

I've been thinking a lot about natural selection, lately -- though less as a
natural phenomenon, and more as a generic algorithm. There's a long
and enduring stream in AI research and development that falls under the general
rubric of "evolutionary computation", which implements Darwinian selection as a
generic problem-solving algorithm. In the subfield of "genetic programming", 
which is the one with which I have the most 
[practical experience](http://roper.eschatronics.ca),
this means evolving populations of programs as a way of discovering means of
carrying out certain tasks. This works, comparatively, quite well when the task
is intractable in the face of less stochastic programming methods -- typically,
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
it as a form of machine intelligence! There's something sublime in this, and
it's genuinely fascinating to behold.

![Sacculina](/img/Haeckel_Sacculina.png)

## Coevolution and Parasitism

Anyway, lately I've been studying ways of engineering co-evolution. 

Instead of measuring the evolving population against some static, a priori
measure of fitness, coevolutionary algorithms evolve the selection mechanism
along with the population it selects from. This is typically done by having a
_second_ population exert selection pressure on the first, and vice versa.
Sometimes this is compared to the relation between host and parasite
populations, or predator and prey. The parasite poses problems to the host, and
itself has to adapt to this task. The host tries to solve these problems in
return.

There's a few ways this can go. The two populations can lock into an "arms
race", each adaptation accelerating the evolution of its opponent. It's also
possible for the two populations to _collude_, learning to pose as little
challenge as possible to one another, settling into a sort of oligarchal
mediocrity. An especially common outcome, however, is for the two populations to
simply _disengage_. 

It was a paper by John Cartlidge and Seth Bullock, entitled
[Combating Coevolutionary Disengagement by Reducing Parasite Virulence](/data/parasite-gp.pdf)
that initially captured my imagination, on this topic. "Coevolutionary
disengagement", they begin, 

> occurs when one advantaged population
> outperforms another to the extent that conspecifics become indistinguishable from
> one another interms of fitness. At such times, coevolving populations become
> decoupled, and se-lection acts indiscriminately causing the system to drift,
> often with deleterious results

The word "outperforms" can be a bit misleading, here. It's not that one
population is doing _better_ than the other, in any objectively meaningful
sense. Only that it has lost any means of telling its counterparts apart. A
teacher whose tests have become so impossibly difficult that all of her students
uniformly fail, for example, is "outperforming" the students, in this sense --
but in this sense alone.

![genpong](/img/pong.png)

Or to take another example, and one you can experiment with
a bit more freely, imagine
[(or implement)](https://github.com/oblivia-simplex/genpong)
two populations of pong players -- one of which always
plays the right side of the table, and one of which always plays the left. Let's
say that the fitness function is something like "the number of games won".
Players that win against the opposing population go on to breed (at least
probabilistically) and ones that lose, don't. Now, suppose we've reached a point
where the left population defeats every single right-side player with equal (and
high) probability. At this point, whatever selective pressure that the left side
imposed on the right is lost -- and vice-versa. The two populations are no
longer able to distinguish between one another's members, and, as a result, the
fitness landscapes that the two populations find themselves upon have been
flattened to a plane. Variation continues to occur, but it is now a purely
stochastic process, a random walk. With selection no longer playing a role,
[genetic drift](https://evolution.berkeley.edu/evolibrary/article/evo_24) comes
to dominate the evolutionary process. Adaptation has stopped, and any
"intelligence" that the system might have exhibited gives way to a kind of
free-floating delirium.


## Radical Postures and Memetic Drift 

It's interesting to look at the relationship between academic philosophy and its
outside through this model: entire discourses -- or "discursive populations" --
that are no longer sensitive to any selective pressures from the outside.
Or none, at least, whose selective criteria are relevant to philosophy's own
"fitness". The sciences, from academic philosophy's perspective, have coalesced
into an opaque monolithic block, whose harmful radiation is warded off by cries
of "scientism". Political realities, for their part, are smoothed into
a small set of opaque, featureless banners. And so on. 

Of course, these discourses continue to mutate, and _some_ sort of selection 
still occurs, in the blind caprice of committees -- mechanisms that discursive
trends can certainly game, but not really _as_ philosophy. "Memetic drift"
settles in -- a random walk through academic memespace, whose paths we
can afterwards describe only in terms of fashion.

This might be an interesting way of framing political disengagement, too. I'm
not talking about apathy or listlessness here. Disengagement, in this set, can
be passionate. It can even be romanticised -- an angelic posture
so intense, so virulent, that no adversary can measure up to it.
Everything is equally unacceptable. A sort of polarization takes place, but one
that seems less and less like an actual struggle, and certainly has less and
less of an effect on its environment (including, of course, its adversarial
host). A parasite that, for all its virulence, is no longer able to steer the
evolution of its host, in any relevant way, is ill-suited for politics, a craft
where your instrument is your adversary.

If disengagement is the Scylla, collusion's the Charybdis -- a situation where
the selective pressure each population exerts on the other is _softened_
to the point of insignificance, rather than impossibly hardened. The ultimate
effect on the process is the same: both collusion and disengagement amount to
a surrender to drift. Complacent apathy and holy radicalism mirror each other, 
here. Any chance of sculpting the adversary's political
memeplex is lost, along with any chance of adapting to their tactics.
All that's left is a sort of delirium, steered only by the vagaries of the
attention economy. 

