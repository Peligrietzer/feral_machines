# Hello, World!

Back when the philosophical blogosphere was really booming -- which, let's say
was between 2005 and 2013, going by
[K-Punk](http://k-punk.abstractdynamics.org)'s lifespan -- I was spending most
of my time wrangling a brood of young kids and a couple bouts of grad school. It
was a silver age for the internet, but I spent most of that time on the
sidelines, one or two false starts aside.

After 2013, it seemed, the old enthusiasm for the medium had faded. Maybe it
was just a matter of pacing. Social media -- facebook & twitter, chiefly --
drew the discourse into its acceleration chambers, and as we became accustomed to
its frantic speed and density, I suppose the blogosphere of a few years prior
just didn't scratch the itch. The mood now, at least from here, feels a bit like
a dopamine [hangover](https://www.youtube.com/watch?v=DikWW4pOehk). What I seem
to feel nowadays, when I open up facebook or twitter, is a kind of dutiful
weariness. I'm glad those media are there, as a way of keeping in touch with
friends that would otherwise be hard to reach, but the joy of the media
themselves is just... *gone* for me. I can never really drum up a motive to post
there, anymore.

This isn't at all a bad development. In many ways, it comes as a relief -- *that
frozen moment when everyone sees what's on the end of every fork*. It seems,
among other things, a good incentive to take another stab at blogging...

---

(Why does that line of Burroughs' (or of Kerouac's, as remembered by Burroughs?) 
feel so appropriate here? Why the "everyone", the "every fork"?
And why am I writing about my disaffection with
"social media" as if it's anything but an idiosyncratic itch -- as if I'm
just giving voice to a Zeitgeist, or, at least, to some
[20,000 people standing in a field](https://www.youtube.com/watch?v=DikWW4pOehk).
Seems kind of presumptuous.
I'm not really sure if I'm just -- selectively -- picking up
on a mood in the air, or casually generalizing from a sample set of one.
But, [I suppose, at least, I'm not alone](https://thelastinstance.com/posts/regulate/)
in this sentiment. Whatever it is, there's enough of it going around
to get some hope of a blogosphere rolling, again.)

---

Another reason for doing this is just that I *miss writing*. I left the
humanities in 2013, for various reasons, and in 2014 started shifting
towards tech. I rediscovered a joy in programming that I hadn't touched
since I was a kid coding in BASIC, and learning that I could indulge in
that *and* escape grinding poverty was a delightful revelation. I still
do love programming, and computer science as a field of research, but
*writing*, writing prose, is something I'm starting to want back in my
life. 

## P'log, the Hairless Yak

Now, as much as I enjoy writing, I quite like programming, too, and
there's nothing quite as satisfying
as a [smoothly shaven yak](https://www.youtube.com/watch?v=trXjZ70ab1Q). 
So, when it came time to choose a blogging
platform, I decided, fuck it, I'll just write my own.
And, to make it interesting, I figured I'd
do it in [Prolog](http://swi-prolog.org).

Prolog is a beautiful and elegant language, it's like programming with
[sequent calculus](https://en.wikipedia.org/wiki/Sequent_calculus). 
I'd done a little bit of basic, and very academic, work with it before
-- writing parsers and interpreters and so on, for a toy language --
but I'd never actually used it for anything immediately practical.
But I remembered Annie Ogborn singing its praises as a web development
language in the 
[##prolog](http://irc.netsplit.de/channels/details.php?room=%23%23prolog&net=freenode) 
channel on Freenode, and, since I'd never
actually *done* any serious web development (aside from a brief stint
as the web developer for the archives of Slocan City, which it wouldn't be fair
to call a "silver rush ghost town", but which it wouldn't be accurate not
to -- but that's a whole other story) I figured, why not start with
Prolog?

This turned out to be a delightful choice. I spent a few days hacking together
an extremely minimalistic blog server in this language, which you can find the
code for [here](https://github.com/oblivia-simplex/plog). Annie's 
[tutorial](http://www.pathwayslms.com/swipltuts/html/index.html)
has been *immensely* helpful in finding my way through this project.

"P'log" is the ongoing result of that coding binge -- a binge that
was, in fact, 
the first time I'd just sat down and coded for *fun* in several weeks, 
(the executive function deficit and brainfog that
go hand in hand with post-surgical recovery are nothing to be sneezed at). 
I'll keep tinkering with
it, but I feel like it's gotten to the point where I have things the
way I like them. If you'd like to use it for your own site, please,
be my guest. It's all under the [GPL](/content/info/gpl.md).


## Feral Machines


My research in the field of computer science has orbited around two
principal focii: machine learning, on the one hand, and
information security, on the other. I wasn't *exactly* sure why I'd
picked those two domains when I signed up for my MCS, other than that
found myself fascinated with each (both just seemed *really cool*),
and that there was something intrinsically intriguing about those
domains where *programs* -- those paragons of clarity and
transparency of purpose -- were rife with surprises. 

My interest in security zeroed in on what Halvar Flake named
["weird machines"](https://en.wikipedia.org/wiki/Weird_machine).
These are virtual machines that supervene, spontaneously, and without 
having ever been *designed*, on deliberately constructed computational
systems. "Exploitation", at least in its most interesting instances,
is just the discovery, and then programming, of some such "weird machine".
It would take me too far into the weeds of this already weedy post to
go into too much detail, here, but it's something I'll certainly come
back to. 

My interest in machine learning, meanwhile, had converged on the
domain of evolutionary computation, and program synthesis through
genetic programming. Genetic programming is the exact art and subtle
science of breeding *populations* of instruction sequences in
systems that implement the essentials of Darwinian natural selection
(as well as various, non-standard models of evolution, as we see fit). 

My grad research brought these streams together, and explored the *evolution of weird
machine code* -- [ROP](https://en.wikipedia.org/wiki/ROP) chains, in particular
-- culminating in 
[Urschliem in Silicon: Return Oriented Program Evolution with ROPER](http://eschatronics.ca). 
As that project developed, the intuition guiding it started to crystallize -- a
sense of how untamed -- *undesigned* -- the computational capacities of our
systems really are, leaking through our rather pragmatic abstractions, and
exposing a weird, internal wilderness that's ripe for evolutionary exploration,
in all its acephalic genius.

This was all in the back of my head, I think, when I picked the title 
for this blog, on what felt like a bit of a whim.
But I think it condenses at least a few of the themes that interest me, 
and which I anticipate exploring here, regularly. There's a whole
chain of associations, it seems to me, that links together -- in 
some vague, hard to place sort of way -- so many of the things I've
been (and remain) interested in writing about -- both inside and outside
of computer science. Epistemological obstacles, emergent memetic ecologies,
xenofeminist ethics, weird machines and hidden logics, blind spots both
accidental and inevitable, surrealist poetry, 
leaky abstractions and their exploitation...
There's a certain 
["vibe" to this canon](http://www.glass-bead.org/article/a-theory-of-vibe/?lang=enview),
I feel, though I'm not sure I can make it precise. "Feral machines" 
certainly doesn't sum it up, but it seems as a good a bearing as any. 
