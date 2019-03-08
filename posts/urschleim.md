
![img](/img/AI_ooze_transparent.png)

## The Story So Far...

Over at Conflated Automatons, Adam has posted a
[third installment](https://conflatedautomatons.wordpress.com/2019/02/15/just-like-reifying-a-dinner/)
of a series on coding, ambiguity, and "ontological slime",
responding to
[this post](https://thelastinstance.com/posts/digital_goop/)
over at The Last Instance -- which, in turn, was replying to 
[this one](https://conflatedautomatons.wordpress.com/2019/01/08/heaps-of-slime/),
again by Adam.

The theme connecting these posts is that penumbra of the vague, the 
inelegant, and the arbitrary that creeps up on us where programs
interact with the "outside world", and the ontological decisions that
programmers are called upon to make when navigating that murky terrain.

This experience isn't unique to programming, of course. "There are many
times in science and engineering," in general, Adam notes,

> when we can not solve problems using universal rules. William Wimsatt names
> these conditions of highly localized rules "ontological slime", and the
> complex feedback mechanisms that accompany them "causal thickets".


## The Slime Is Seeping from Inside the House

While the emphasis in Adam's first post are the little decisions by which
software engineers collapse ambiguity by fiat -- abjuring the ambiguity
of [sorites problems](https://plato.stanford.edu/entries/sorites-paradox),
for example, by mapping heaps and herds and so on to unambiguous formal 
structures -- 
Dominic's response at [The Last Instance](https://thelastinstance.com),
"[Digital Goop](https://thelastinstance/posts/digital_goop)",
draws attention to how

> reification in such cases is not a matter of spiriting away the fuzzily
> empirical particularity of the domain into a crisp, frictionlessly powerful,
> abstract notion. It is rather the construction of a machine that mediates
> between domains: a "thingifier" which adapts one sort of thingliness for the
> purposes of another. [...] It is simultaneously a theory about the world, and
> a theory about the means at hand for dealing with the world.

Software often becomes "slimy" -- that is, a tissue of entangled local
compromises -- simply as a consequence of dealing with a rather slimy world.
This insight carries over into the third installment in this dialogue, with
Adam's [most recent post](https://conflatedautomatons.wordpress.com/2019/02/15/just-like-reifying-a-dinner/):

> Especially in software, and its everyday entanglement with human societies and
> institutions, general rules are an exception. Once you find them, they are one
> of the easy bits. Software is made of both planes of regularity and vast
> quantities of ontological slime.

But where things get _particularly_ interesting, I think, is when we observe
that this "sliminess", or recalcitrance to generality, isn't just a 
consequence of software's congress with its other -- as if, in its own
Platonic abode, computation would be able to grasp itself clearly and dryly.

[ -- transition needed -- ]

### The Limits of Static Analysis

This observation actually runs up against the Halting Problem, and the art of
[static program analysis](https://youtube.com/watch?v=POvX4hYIoxg), 
in interesting ways. For any non-trivial property,
it is strictly _impossible_ to concoct a "universal rule" that would let you
partition the universe of programs into those which have that property, and those
which do not. This is the upshot of 
[Rice's Theorem](https://en.wikipedia.org/wiki/Rice%27s_theorem),
an corollary of Turing's Halting Theorem. This doesn't mean that we can't 
concoct rules -- or algorithms -- that still do a _pretty good job_ of 
deciding, for a given program P, whether or not P exhibits some interesting
property. But "pretty good", here, cannot mean certain or universally applicable.
There exist a great many methods of static analysis, but every single one of
them represents a certain compromise with this impossibility at the heart of
computation: they may be

1. unsound (prone to false positives),
2. incomplete (prone to false negatives), or
3. occasionally, and unpredictably, non-terminating.

In effect, even our rules for analysing that most general of things in computer
science -- the _program_ -- are insuperably partial, or "slimy". It's not just
when it's forced to deal with "the real world" that computer science gets
tangled in the thicket of uncertainty. Like someone -- was it Hegel? -- once
said about the concept: _computation wants nothing more than to grasp itself, but
it ever stands in its own way_. 

### Compilers and Ontology

Though Adam doesn't mention these principled limits to universality in computational
reflexivity, the theme of reflection does come up in an interesting way in his
discussion of compilation:

> Hopper invented the first compiler: an ontology-kneading machine. By providing
> machine checkable names that correspond to words in natural language, it
> constructs attachment points for theory construals, stabilizing them, and making
> it easier for theories to be rebuilt and shared by others working on the same
> system. Machine code – dense, and full of hidden structure – is a rather slimy
> artifact itself. Engineering an ontological layer above it – the programming
> language – is, like the anti-sorites, a slime refinement manoeuvre.

What does "full of hidden structure" mean, here? Why is it hidden, and what
is it hidden _from?_ Well, we know, already, that the tangle of structure
in a piece of code is at least hidden from any universal and _a priori_ viewpoint.
It's never _unknowable_, but our knowledge of what structures lie within
must be won locally, in a case by case fashion.

I think it's quite helpful to think of a compiler as a mapping from a
scaffolding for "theory construals" -- a programming language, outfitted
with its system of abstractions: functions, datatypes, and so on -- 
to a domain on which these abstractions are traced, but which they 
do not, necessarily, _constrain_. Of course, it's the source language
and its compiler's job to ensure that the behaviour of the dark ocean
onto which these abstractions are mapped is indeed constrained by the
abstractions in question -- whether through compile-time checks, or
just by providing the programmer with arcane warnings regarding
[undefined behaviour](http://blog.llvm.org/2011/05/what-every-c-programmer-should-know.html).
The compiler reasons about its target's dynamics so that you, the source
code programmer, don't have to. It facilitates and remediates a threshold of 
competence, and _creates_ a hierarchy of "ontological levels", 
in Wimsatt's sense.

# TODO

- Elaborate Wimsatt's sense of "ontological levels",

- It may sound strange to speak of "abstractions" and "ontological levels" more
or less interchangeably. Explain this.

## Yeggogology

But mistakes happen, and sometimes our carefully traced abstractions "leak",
with a consequent leakage between ontological levels. 

Interestingly, William Wimsatt, in 
["The Ontology of Complex Systems: Levels of Organization, Perspectives, and Causal Thickets"](https://pdfs.semanticscholar.org/593c/cfacbef43e2bca905b78df234ff32a1ced58.pdf) --
the source of the ontological categories with which this discussion, from its
beginning on Conflated Automatons onwards, has been framed -- draws his
paradigmatic illustration of the phenomenon of ontological "level leakage" 
from the domain of software engineering: 

> The ways in which we exploit "level leakage" to gain access to other levels
> became much clearer to me through my involvement in 1979-81 in helping to
> program a custom ROM module for the Hewlett-Packard HP-41C programmable
> calculator. The calculator was designed to be programmed in RPN, (for "Reverse
> Polish Notation"), a sort of assembly-level language which allowed direct
> manipulation of program instructions, numbers and alphabetical characters in a
> controlled regionof the calculator's memory, preventing access to other regions
> of memory used by the calculators "system software", on the other side of a
> "curtain". A "bug" in the definition of some of the keyboard functions on some
> early calculators gave unintended ways of creating new "synthetic instructions"
> which gave ways of moving the "curtain" and of directly manipulating the
> contents of control registers behind the curtain on all HP-41 calculators,
> whether they had that bug or not. This led to a new machine-specific discipline,
> called "synthetic programming", which gave the synthetic programmer control over
> many things on the HP-41 that Hewlett-Packard engineers never intended (e.g.,
> individual elements in the LCD display, and individual pixels in the printer
> output, and the ability to do all sorts of bit manipulations to compose new
> kinds of instructions). ‘Synthetic programming’ thus gave new capabilities, and
> sometimes striking increases in efficiency, speed or power. On the down side, it
> also gave new and dangerous ways of "crashing" the calculator, and exploiting
> this new resource required much greater knowledge of the details of the machine,
> such as the Hexidecimal code for all machine instructions, and greater knowledge
> of how they worked, and how they interacted with the hardware. See the 500+ page
> PPC ROM User's Manual, 1981 for the section on the history and description of
> "Synthetic Programming" and also a later (1982) book of that same title by its
> main developer, William Wickes.

Wikipedia's entry on [Synthetic Programming (HP-41)](https://en.wikipedia.org/wiki/Synthetic_Programming_(HP-41)) elaborates a little on the
technique:

> Synthetic programming uses a bug in the calculator firmware to enter those byte
> sequences as a sequence of other instructions, then partially skipping halfway
> through the first instruction, so that the calculator believes the end of the
> first instruction is actually the beginning of a new one.

![Wickes](/img/synthetic_programming_on_the_hp-41.jpg)

I haven't yet been able to find a copy of Wickes' book (pictured above), but the
level of nerd sniping evident on its back cover alone -- with its Carrollian
paen to calculator hacking -- has me at its mercy.

![Wickes](/img/synthetic_programming_on_the_hp-41--rear.jpg)

Transcription:

<a name="keyboardlocky"></a>

```
KEYBOARDLOCKY

'Twas octal, and the synthetic codes
Were scanned without a loss.
In and out of PRGM mode,
Byte-jumpers nybbled the CMOS.

"Beware o' STO c, my son,
The MEMORY LOST, the keyboard lock.
Beware the NNN, and shun
The curious phase 1 clock."

He took his black box codes in hand
Long time the backwards goos he sought;
The secret beast from Aitchpee land--
All searches came to nought.

In demented thought he stood, and then:
The goose, with LCD's alight,
A leap for every LBL 10,
Came honking left-to-right!

STO b! STO d!, and RCL P!
His keyboard went clickety-clack.
With the proper code in number mode
The goose came flapping back.

"And hast thou found the phantom fowl?
Come to my arms, my binary boy.
Let Corvallis hear us how
As we chortle in our joy!"

'Twas octal, and the synthetic codes
Were scanned without a loss.
In and out of PRGM mode,
Byte-jumpers nybbled the CMOS.

--Apologies to Lewis Carroll

```

Spelunking this rabbithole has gotten me nerd-sniped by some truly delightful
findings -- my favourite of which is the term that Russian hackers (stop)
concocted to describe their forays into programmable calculator exploitation in
the mid-80s: *yeggogology*. Wikipedia offers the following explanation:

> This series of calculators [i.e., ones using the B3-34 instruction set]
> was also noted for a large number of highly
> counter-intuitive mysterious undocumented features, not unlike the "synthetic
> programming" of the American HP-41, which were exploited by applying normal
> arithmetic operations to error messages, jumping to non-existent addresses and
> other techniques. A clever step away from the documented path would often
> cause some highly unusual things. [...] A number of respected monthly
> publications, including the popular science magazine "Nauka i Zhizn" ("Science
> and Life"), featured special columns, dedicated to optimization techniques for
> calculator programmers and updates on undocumented features for hackers, which
> grew into a whole esoteric science with many branches, known as "errorology"
> (Russian "еггогология," transliterated "yeggogologiya"). The error messages on
> those calculators were intended to appear as the English word "Error", which
> to the Russians looked like a meaningless "ЕГГОГ" (YEGGOG).

How this word is not on every red-blooded hacker's lips is a mystery to me. The
closest equivalent term I can think of would just be "hacking", in its truest
sense, though it casts too broad a net (even without rehashing moribund
90s debates on the merits of "hacking" vs "cracking"). 
["The Science of Insecurity"](https://www.youtube.com/watch?v=3kEfedtQVOY)
works, but
feels like a description _in search_ of a name. But we do, at least, have a
perfectly good term -- and, better, a concept -- for the _subject matter_ of
yeggogilogical research: 
["weird machines"](https://www.cs.dartmouth.edu/~sergey/wm/).

### Weird Machines

The term seems to have been first introduced by
[Sergey Bratus](https://www.cs.dartmouth.edu/~sergey/hc/rss-hacker-research.pdf),
but has received its most systematic definition through the work of 
[Halvar Flake](https://ieeexplore.ieee.org/ielx7/6245516/6558478/08226852.pdf)
(aka Thomas Dullien).


### Leaky Abstractions (recap)

The exploration and programming of weird machines is possible, generally
speaking, because abstractions -- or "ontological levels", in Wimsatt's sense
-- leak. Software engineers, in fact, are fond of citing
[Spolsky's Law](https://www.joelonsoftware.com/2002/11/11/the-law-of-leaky-abstractions/)
on this subject: 

**All non-trivial abstractions, to some degree, are leaky.**

It's more of a rule of thumb, really, than a law of computation (in the
sense that, say, Rice's Theorem gives us a "law of computation"). But
exceptions are few and far between, and, for any particular case, it's
good practice to assume the truth of Spolsky's Law unless the contrary
can be proven. 

## Smashing Function Ontology for Fun and Profit

Let's take the idea of a "function" or "subroutine" in an imperative language,
like C, for an example. What's the "theory of the function" that the programmer's
working with? Without trying to get too formal, it's something like this: by
calling a function, I temporarily hand over control to the code in the function
definition. The computer executes that code, and then _returns_ control to the
instruction immediately following the function call. 

In the program below, for example, the control flow starts at the beginning of
the function main(), and shortly afterwards, jumps to the code in the definition
of hello(), and then -- after a couple more calls to strcpy() and printf(), a
couple of functions from the standard libraries, **string** and **stdio**,
respectively -- returns to the line immediately following our call to hello(),
to inform the user that they have, indeed, been greeted.

<a name="code_example"></a>

```C
#include <stdio.h>
#include <string.h>

void weird(void) {
  printf("ph'nglui mglw'nafh Cthulhu R'lyeh wgah'nagl fhtagn\n");
  return;
}

void hello(char *name) {
  char buffer[10];
  strcpy(buffer, name);
  printf("Hello, %s!\n", buffer);
  return;
}

int main(int argc, char **argv) {
  if (argc < 2) {
    printf("Usage: %s <your name>\n", argv[0]);
    return 1;
  }
  printf("This program is going to greet you.\n");
  hello(argv[1]);
  printf("You have been greeted.\n");
  return 0;
}
```

Now, since function calls can be nested -- see the calls to strcpy() and printf()
inside hello(), for instance -- our system of "bookmarks that tell us where to
resume execution after running each function is naturally representable as a 
stack. Each call **pushes** a new "bookmark", or return address, to the top of
the stack, and each return **pops** the address from the top of the stack, and
tells the CPU to jump to that address by writing it to the CPU's "program counter".
This ideal stack of addresses is what we call "the call stack". The call stack,
in this sense, forms part of the (more or less spontaneous) "theoretical" 
(in
[Peter Naur's sense of the term](https://news.ycombinator.com/item?id=10833278)
)
grasp that programmers have of the control flow structures they're building. 
It's natural, and, usually, helpful to think of nested subroutines or functions
as forming a "stack", since we must complete the function we most recently
embarked upon before resuming the next one down -- from which we embarked.

And, indeed, compilers -- GCC, for example -- are guided by this very idea
in their implementation of function calls. But with a crucial complication:
in most implementations, the call stack is interleafed with the data stack,
where the locally scoped variables used in each function are stored -- like
the **char buffer[10]** variable, which belongs to **hello()**'s scope, 
in the [above example](#code_example).

![stack frame](/img/stack_frame.png)

From the perspective of the unwary programmer, call stacks and local
variable scopes are two distinct abstractions, with no direct means of
interaction, beyond the mechanism of call-and-return that articulates
them. (When we return from a function, we return not only to the
address from which that function was called, but -- at least in most 
modern languages -- to the lexical environment of the caller.)

On the level of machine code, however, these abstractions have a way
of leaking into one another, and, unless great care is taken to secure
the system, become causally entangled with one another to disastrous
effect. 

Let's go back to [our example](#code_example), now, and compile it. 
On a Linux or Unix system, with the **gcc** compiler installed, you can do this
like so:

```
$ gcc -fno-stack-protector \
    -zexecstack -g -O0 -m32 -static \
    hello.c -o hello
```

The command line options you see here tell gcc to omit a few modern 
security features (stack canaries and W&oplus;X, in particular), as well as
a few compiler optimizations, so as to keep this illustration nice
and simple. It also tells the compiler to include some helpful debugging
information, and to target only the 32-bit subset of the x86_64 instruction
set, which makes things a bit simpler still. We're also going to tell the
compiler to statically link any required libraries, again, for the sake o
simplicity. You can run it now, if you like:

```
$ ./hello Lucca
This program is going to greet you.
Hello, Lucca!
You have been greeted.

```

If your name happens to be ten characters long or longer, however, things
will have gone very differently for you. 

```
$ ./hello Luccaaaaaaaaaaaaaaaaaaaaaaa
This program is going to greet you.
Hello, Luccaaaaaaaaaaaaaaaaaaaaaaa!
Segmentation fault (core dumped)
```

We only allocated 10 bytes to the **buffer** array in the **hello()**
function, after all, and so the excess characters are written to stack
memory *beyond* the bounds allocated to **buffer** -- spilling over into
the call stack with which the data stack is interleafed. When it comes
time to "return" from the function, hello(), the CPU fetches the return
address -- the "bookmark" -- from the stack, and finds, instead:
**0x61616161**, which, non-coincidentally, is just the bytewise representation
of "aaaa".


```
$ gdb ./hello
Reading symbols from ./hello...done.
(gdb) run Luccaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
Starting program: /home/oblivia/hello Luccaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa
This program is going to greet you.
Hello, Luccaaaaaaaaaaaaaaaaaaaaaaaaaaaaaa!

Program received signal SIGSEGV, Segmentation fault.
0x61616161 in ?? ()
(gdb) print $eip
$1 = (void (*)()) 0x61616161
(gdb) info stack
#0  0x61616161 in ?? ()
#1  0x61616161 in ?? ()
#2  0x61616161 in ?? ()
#3  0xffffc900 in ?? ()
Backtrace stopped: previous frame inner to this frame (corrupt stack?)
(gdb) 

```

In a certain sense, data and code are one and the same, and the fundamental 
problem of cybersecurity is drawing a line of demarcation between the two
categories. The ideal state of affairs is one where the data that the program
receives as input steers the program's execution, but only along meticulously
designed pathways. The data, in this way, can be seen as "code" for a very
limited state machine, such as the one shown below. Here, passing the empty
string (denoted &epsilon;) as input sends us to the "Usage Instructions" state,
while -- ideally -- passing a name as input sends us to the "Greeting" state.

![fsm1](/img/hello-fsm.png)

This state machine represents a tiny ontological level of its own, abstracted
away from the general purpose computer that thrums below. But this abstraction
springs a leak the moment we attempt to pass the application a name containing
10 or more characters. The "function" abstraction, which the programmer relied
upon to construct the "Hello Machine" abstraction, is broken the moment the
input data overwrites the return address pointer on the stack -- the exact
structure of which the programmer may have given little thought. Its foundations
in the "Structured Programming Machine" undermined, the ontological
plane of the Hello Machine drops out from under us, and we are cast into
what we call a "weird state" (illustrated below).

![fsm2](/img/hello-fsm-shoggoth.png)

But this isn't the end of the story. The underlying machinery is still running,
and this weird state opens onto a virtually boundless horizon of possibility.
If we overwrite the return address with "aaaa" then, it's true, we won't have
much to look forward to. But why not take advantage of the fact that the CPU
is prepared to treat whatever it finds at that place on the stack as an
_address_? 

And, since we have allowed stack memory to be executable, like it was in the
90s, with the compiler option "-zexecstack", we can even include some machine
code of our own as part of the "name" string, and, once we have determined its
address, "return" to that. This is the substance of the classic buffer overflow
attack strategy made famous by Aleph One's 
[Smashing the Stack for Fun and Profit](http://phrack.org/issues/49/14.html),
in the 49th issue of Phrack.

![smashing the stack](/img/stack_frame_attack.png)

### The Geometry of Innocent Slime on the Bone

It was in response to this sort of attack that the security measure known
as W&oplus;X ("write xor execute") was introduced.

You'll have noticed, in our [example](#code_example), that there is no obvious
way of reaching the function named **weird()**. For all intents and purposes, 
it looks like dead code. But (since we disabled compiler optimizations) it's
still there, and has an address:

```
$ nm hello | grep weird
08049b05 T weird
```

(Here, we dumped the hello binary's namespace with nm and searched for the name
"weird" with grep.)

With a bit of trial and error (or patience and calculation), we can determine
the exact offset at which to place this address (in raw, little-endian format,
which in the bash shell can be achieved by putting **$'\x05\x9b\x04\x08'**)
so that when the CPU goes to fetch the return address of the call to hello()
from the stack, it finds 0x0849b05 instead, and continues on its way, never
the wiser.

```
$ ./hello 1234567890123456789012$'\x05\x9b\x04\x08'
This program is going to greet you.
Hello, 1234567890123456789012!
ph'nglui mglw'nafh Cthulhu R'lyeh wgah'nagl fhtagn
Segmentation fault (core dumped)
```

The "Segmentation fault" at the end, here, only comes about because, when
the CPU goes to fetch the return address from the stack upon reaching the
end of weird(), it finds nothing that points to executable code. We can
remedy this by putting _another_ address at the end of our "name". For now,
let's just put the address of weird() again:

```
$ ./hello 1234567890123456789012$'\x05\x9b\x04\x08'$'\x05\x9b\x04\x08'
This program is going to greet you.
Hello, 1234567890123456789012!
ph'nglui mglw'nafh Cthulhu R'lyeh wgah'nagl fhtagn
ph'nglui mglw'nafh Cthulhu R'lyeh wgah'nagl fhtagn
Segmentation fault (core dumped)
```

We can, in fact, put any sequence of addresses that we like. 





### Urschleim in Silicon

Interestingly, what nudged Adam's analysis into this reflective posture -- one
bearing on the ways in which not just the world, but code itself, is slime for
code -- was Dom's reply, 
[Digital Goop](https://thelastinstance.com/posts/digital_goop/), which
concludes with this intriguing analogy:

> The way forward may be to see slime itself as already code-bearing, rather as
> one imagines fragments of RNA floating and combining in a primordial soup.
> Suppose we think of programming as refining slime, making code out of its codes,
> sifting and synthesizing.


This got me thinking about the (rather pulpy) imagery that I used when I
introduced [ROPER](http://roper.eschtronics.ca), imagery that made it into the
title of my thesis: *Urschleim in Silicon: Return Oriented Program Evolution
with ROPER*.
