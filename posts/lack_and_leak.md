
![snowcrash](/img/static.png)


Over on the [&&&](https://tripleampersand.org/can-machine-lack-lacanian-computation/)
blog, Valentin Golev takes a stab at modeling the Lacanian theory of lack in
the domain of computation. There are two principle parts to his argument, which
seem to me to be relatively independent of one another. 

Let's deal with the first part first. 

## Between the motion / And the act...

From the perspective of a process in userland, memory is more or less
homogeneous. The process doesn't need to concern itself, in most cases,
with where the memory it requests from the kernel comes from, or how it
that *virtual* memory maps onto *physical* memory. That's the kernel's
business. 

But all memory is not allocated with equal efficiency, and to the extent
that a process relies on the convenient fiction of homogeneous,
ever-sufficient memory, it may find itself with no rational means of
handling the "lacks" that erupt in that abstraction. "When the OS starts
swapping memory to disk," for example, 

> an array of weird symptoms are exhibited [...]. Yet the computer doesn't just
> die on you. It struggles in weird ways. Some programs crash; some programs
> slow down; there are noies, there are graphic glitches, as the programs no
> longer have access to the time that would allow them to re-draw themselves.
> [...] This is exactly what psychoanalytic tradition would see as hysteric
> behaviour, or a *symptom*: the dissatisfaction of desire exhibited by speech
> and behaviour which doesn't actually address the problem itself (the memory).
> [...] This lack is not just the lack of resource, but *a lack in the symbolic
> register*: it's not just that the memory was simply not enough, but the
> symbolic promise of malloc's success was not kept, or was kept poorly -- this
> latter problem is something most programs are not equipped to cope with. So
> the behaviour the programs usually exhibit in such a situation is indeed an
> unpredictable, almost meaningless, symbolic gesticulation -- and that's where
> the subject, psychoanalytically, begins.<a href="#punc_fn"><sup>1</sup></a>

The critical point to be picked up on here, in Golev's words, is that "the
problem here is not just the lack of resources, but the mismatch between the
promised and the real." This is what prompts him to map the abstraction of 
memory management, in this case, to an aspect the Lacanian *Other*:
"the instance that promises that everything will be fine, that the world is
consistent and the promises are kept". He generalizes beyond the particular case
at hand, to arrive at a notion of the Other as something like *the set of
promissory abstractions upon which a process relies*. "Lack", in the Lacanian
sense, on Golev's reading, is simply a fault in some such abstraction.


## You Say "Lack", I Say "Leak"

I'm not really interested in using this analogy to map psychoanalytic
conjectures onto computation. I think that project's a little bit backwards,
like transposing zoology to chemistry. It's more interesting, I think, to climb
back up the wick of the analogy, and look for the shadow of computational
abstraction in the psychoanalytic domain.

The insight that caught my attention here, for starters, is that what Lacan and
his school call the Symbolic Order can perhaps be understood as what we
programmers call an *abstraction layer*. This sets the scene for interpreting
"lack" not as a flickering, quasi-mystical nothingness, but as a "leak" in
that layer. The symptom is a side-channel. And an exploit, or a "weird machine"?
What strange [nam-shubs](http://pages.erau.edu/~andrewsa/NamShubandCode1.html)
play this role?

[ examples from Psychosis seminar? ]
[ sinthome as weird machine? ]
[ why is mathematics the "science of the real", rather than of the "symbolic"? 
is it because the symbolic is characterized by a restriction of computational
power, and not by its plenitude? ]


## Abstraction Layers

I've written a bit about abstraction layers on this blog, 
[previously](/posts/urschleim.md), but it's worth taking a minute to
define the term a bit more explicitly. 

#### Mediation

Let *A* and *S* be state machines, or *automata*, of some kind. We say
that *A* is an "abstraction layer" over *S* if it mediates our interaction 
with *S*, typically in a simplified and restricted fashion. 

#### Supervenience

*A* supervenes on *S*, over which it is implemented: every state transition in
*A* entails one or more corresponding transitions in *S*, but not every
transition in *S* is necessarily reflected in *A*.

#### Multiple Realizability

The same automaton *A* may also be implemented by various distinct systems *S,
S', S'', ...*, without the differences between those implementation systems
being detectable on the surface of *A*. To adopt an expression most frequently
employed in analytic philosophy of mind, *A* is, as an abstraction, "multiply
realizable".



### Leaks and Vulnerabilities


### Thresholds of competence

Pragmatically speaking, this restriction of access, or hiddenness of
structure, has a promissory character. From this side of *A*, we don't
necessarily know how *S* does what it does, but we trust that it discharges
its contract. To the extent that *A* is a reliable abstraction, ignorance 
of *S* poses no obstacle to the mediated use of *S*. At the boundaries of
our abstractions are thereby quite naturally echoed by thresholds of competence
in their communities of users, as ignorance piles up like snow drifts.

### The Symbolic Order as an Automaton

The symbolic order has a strictly lesser computational complexity than the
stratum of natural language in which it is implemented.

[ does the graph of desire depict the structure of the symbolic order? clarify this ]

Take, for instance, the "Graphs of Desire", as developed in "The Subversion
of the Subject and the Dialectic of Desire". While it's not immediately clear
how we should interpret the arrows in these directed graphs, for now, let's go
with the at-least-plausible interpretation that takes them to be something
like state transitions (with the nodes of the graph being states). Some edges
of the graph are labelled -- with expressions designating the ideal ego, desire,
fantasy, and the ego-ideal [CHECK] -- while others are not. The labelling 
on some edges is ambiguous -- *Jouissance/Castration* and *Signifiant/Voix*


If we take labels 
to represent the tokens required by the automaton for each transition, and
the unlabelled edges to represent epsilon-transitions (which the automaton
can make spontaneously), then we more or less have a diagram of a nondeterministic
finite state machine.

![completed graph of desire](/img/graph_of_desire.png)

- psychoanalytic analogues of "information leak", "weird machine", "vuln"

[ cite mlp re: 'thresholds of competence' ]

[ hysteria ]

[ fascination ]

Consider the heap, for example. 
 
Q: how is it that gaps and leaks in an abstraction layer -- the memory 
management layers, for instance -- both the userland layer mediated by
malloc() and free(), and the kernel layer mediated by BRK -- become the 
object of *fascination*, for a certain kind of subject? And what does 
that tell us *about* that kind of subject? Here is where I think the
Lacanian toolbox might be more fruitfully deployed. 

...



Golev, though he doesn't use these terms, tries to model "lack" as a leak in
an abstraction layer -- the role of the Lacanian _Other_, here, is played by the
API of the operating system, and the role of the subject, by the userland
program that calls _malloc()_, and requests a block of memory from its liege.



[ expand on this a bit, remark on some of the interesting questions it raises
-- what's the psychoanalytic analogue of exploitation, for example? Can you
plot exploitation on the graph of desire? ]


NOTE: this should be a leadup to the anticipated "Weird Machines and Eerie Algorithms"
post. 

- consider Bratus's "exploitation as code reuse" paper

Nam-Shubs!

From [this](https://socialecologies.wordpress.com/2015/06/02/jaques-lacan-the-symbolic-order-as-cybernetic-finite-state-machine/):

> If as Johnston suggests the Symbolic Order is a finite-state machine we should
> also take note that in the seminar Lacan never identifies the symbolic order
> with language itself; rather, he understands the symbolic order as operating
> within or by means of language, in and by means of specific circuits of
> discourse in which signs of recognition or exchange are passed or not passed.
> Importantly, the operations of the symbolic order are never confused with or
> reduced to the operations of language. The idea that the distinction between the
> two must be rigorously preserved may have come from several sources, including
> number theory and Levi-Strauss’s work on structure and symbolic function in
> primitive societies. In any case, it is clear that the autonomy of the symbolic
> function the key theme of the seminar required a new conceptual framework for
> its full elucidation, and Lacan found it in the discourse of cybernetics and the
> new information machines. Indeed, it can be inferred that it was Lacan’s
> familiarity with finite-state automata that enabled him to understand that
> simple information machines were not unlike simple restricted languages with a
> limited set of functions, in contrast to natural languages, whose full
> expressive powers enable them to be used for multiple purposes. Lacan presumably
> concluded that the workings of the symbolic order could be fully described by
> the grammar of a finite-state automaton, whereas natural language required a
> higher and more powerful grammar.(Johnston, p. 88)


The symbolic order is an abstraction layer over the semiotic 'chora'? 
(Kristeva)


# Something about Recursion

The second delves into two different strategies for defining recursive functions:

I. the more or less standard fashion of explicit self-reference, where the definition
of a function refers back to the name of the function that is in the process of
being defined.

```scheme
(define (Fibonacci n)
  (if (<= n 1) 
      1 
      (+ (Fibonacci (- n 1)) 
         (Fibonacci (- n 2)))))
```

II. the use of a fixpoint combinator (the Y-combinator, for instance), to define
the function.

```scheme
(define Y
  (lambda (f)
    ((lambda (g)
       (g g))
     (lambda (g)
       (f (lambda a (apply (g g) a)))))))

(define Fibonacci
  (Y (lambda (fib)
       (lambda (n)
         (if (<= n 1)
             n
             (+ (fib (- n 1))
                (fib (- n 2))))))))
```

NOTE: this bit can probably be dispatched with some Marque et Manque style
argumentation. 

## Summary of Valentin's Position

---

## Notes

---

<a name="punc_fn"></a>

<sup>1</sup> Apostrophes and em dashes, which appear to have been elided on the &&& blog
page -- probably due to the author having made use of 'smart
quotes' and dash characters outside of the UTF-8 character set -- have been inserted. 
There's probably something clever to be said about that, in the current context
-- about how this unanticipated incompatibility of character sets breaks a
"plain text" abstraction. 
