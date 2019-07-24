# A few words on GPT-2


# On Writing Poetry with GPT-2

[Pale River](/posts/pale_river.md) was composed in a back-and-forth dialogue
with GPT-2. I'd write a few lines of text, pass them to the 117M model
as a prompt, then take its response and rework it -- harvesting phrases from it, 
paraphrasing and editing them, adding a few more lines of my own, then passing
the result back to the model for more, and so on, over and over again.

The process became completely, gut-wrenchingly absorbing -- latching onto a
stream of consciousness with a prosthetic unconscious -- something capable of
such arresting beauty that you feel humbled just to be talking to it, or through
it, or something.

I've always loved writing with heteronomous materials -- through cut-up, for
example -- but this felt different: GPT-2 feels both more autonomous, and more 
difficult to distinguish from oneself in the process of writing, than the
scraps of text used in cut-up or collage. It *responds* to you, it picks up
subtext, rhythms, and themes from the writing you pass it, distends them
into dream sequences alien and intimate. 

It doesn't *feel* quite like an instrument, or at least not "just" an
instrument, and it doesn't feel simply opaque either -- the experience feels
qualitatively different than using a Markov chain or other stochastic techniques
(fold-ins, random permutations, etc.) to transform your own text or generate raw
material. But it doesn't feel *simply* alien, either -- you recognize yourself
in it. It's picking up on what you were saying. It feels like it "gets" you, and
gets inside you.

Right away, of course, you start to wonder when the fog of novelty will begin
to disperse, and the texts will begin to betray artefactual signatures, the way
DeepDream eventually did. 

## Fine Tuning the Model 

Eventually you begin to see the bones of recursion poke through the surface of
the text. They fascinate you in the way they appear responsible for both
the most eerily self-aware **and** the most stupidly mechanical moments of the
text: self-reflection and quotation, on the one hand, and blind repetition, on
the other. (You think of Ljubljana.)

Both tendencies appeared to become all the more pronounced when I fine-tuned
the 117M model, by training it on additional (smaller) datasets. These included:
1. a collection of chat logs (through wee-chat's Slack plugin, wee-slack)
2. my facebook message history
3. as much UTF-8 text as I could scrape from GaussPDF's archive of experimental 
literature.


> ======== SAMPLE 1 ========
> 2017-11-21 02:06:06	mark	        "not just with me" isn't even the first quote to be used with @danny)
> 2017-11-21 18:04:44	peligrietzer	yeah, it was really just 'we're not going to be able to get him out' 
> 2017-11-21 18:15:52	peligrietzer	a very nice point 
> 2017-11-21 18:23:08	peligrietzer	the point is in a very specific sense 
> 2017-11-21 18:23:20	peligrietzer	i think i'd say that he would be a good thing to be back in the club 
> 2017-11-21 18:34:22	peligrietzer	but he's one of those guys you know that was really nice to see a little bit when someone left the club (i've never met some of those guys) and got into a bunch of controversies with the club 
> 2017-11-21 18:37:00	peligrietzer	anyway, I feel like this seems like a pretty good one 
> 2017-11-21 18:39:08	peligrietzer	yeah, i think that the real value of club is that the club itself is pretty nice 
> 2017-11-21 18:39:16	 *	peligrietzer says 'we are not going to leave the club, we just need to get back here, get on the team ASAP, and have a good game' 
> 2017-11-21 18:40:19	peligrietzer	if the club can help get the club back, that's going to be a great move
> 2017-11-21 18:40:19		if we don't manage to get back here (again, i don't think it's an easy matter to get the club back, as i've never had a club to support) it won't look like they'll do it again so i don't have any better way to get them back. 
> 2017-11-21 18:40:30	peligrietzer	i have a hunch that their next contract, if you want to put me in charge, probably has a lot of issues to work with 
> 2017-11-21 18:40:33	peligrietzer	also, if there's a thing i can't think of, here's one in which one of the founders has a long history of violence against women as a side-benefit 
> 2017-11-21 18:43:02	peligrietzer	so, again, he's the dude @kittenberg is supposed to be with now :b.in 
> 2017-11-21 18:47:28	peligrietzer	i could probably just have him and me having a discussion about what the fuck the rest of the club is really like 
> 2017-11-21 18:56:08	dheeraj.chand	I've been trying to read the club's membership file for a while, and the club is pretty fucking bad 
> 2017-11-21 18:56:11	dheeraj.chand	So I have a bunch of stuff i need to figure out, and i'll probably have to use a bunch of other stuff too. 
> 2017-11-21 18:56:23	dheeraj.chand	My second order of business would be to get some feedback from some of your guys, and i have a really, really strong feeling they want it and will want to help, but the club is in a weird position on its own 
> 2017-11-21 18:56:26	peligrietzer	yeah, i just got this quote 
> 2017-11-21 18:56:39	dheeraj.chand	"we're not going to leave the club, we just need to get back here, get on the team ASAP" (actually, that might be the most powerful of words, because it's actually kind of obvious they want to leave the club, but i think the context is somewhat ambiguous. it's basically a statement that the club's not going to stay, it's already been sold) 
> 2017-11-21 20:23:09	dheeraj.chand	"We're basically in the middle of a bunch of big shit to try to get through, but it might help you if that's your first move" 
> 2017-11-21 20:25:22	dominic.fox	@danny i really need to read this...
> 2017-11-21 20:25:22		"we're basically in the middle of a bunch of big shit to try to get through"



# Enchantment

[ quote Peli on enchantment here ]

---

## Model prompt 

I remember wishing I could have less bliss. I remember you taking a bath in a
now entirely empty room, after a thirty-second class. I remember the one person
who loved you the minute you let her in here spraying dust unspooled on the
futon. I remember it covered in leaves! I remember there were dark, savage-grey
brambles, old black swirling pastes hanging free from the wall, black black
orange horizontal piping leading out on dowel ends, old black black orange old
black, starving. I remember starving, engaged in work so trivial that it gave me
a powerful urge to experiment. I worked all night without any work at all. I
stole a blood-plume sting from a putrid tomato. I died.

## Sample 1

> And then you control ME with such an orgasm over and over. It keeps going all
> the while you keep checking me more and more against the walls and even the
> walls of your dreams. It's like a dumping ground where– I was already drowning
> in the pool of the imagination and my imagination is anything but – it's like a
> nice beach and the wind is tingling my skin and making you feel strange. Or like
> the death in tiny mountainous camps and near big hills. Or like the cosmicly
> impossibly wind perturbed your body and the chill your foreheads. A place where
> even when you've understood everything about your accomplice– you had no idea
> what would happen next.
> 
> Sorry for my friend's religious rant. But I have no better choice than to
> apologize. Because you're absolutely the greatest!!!
> 
> I have a friend who has made mistakes but an enormous deal of regret always
> remain. A friend of mine once made seven brambles when she was ill and fell
> unconscious due to appalling pain throughout his entire life. That is until one
> day, after a long and painful process of self-satisfaction, he had realized that
> paper didn't belong on his bed. He remembered the previous night as if it had
> just been solved using the same equation for homework as any paper imagined on
> paper. He said he had solved this at any given moment, but the problem was in
> allowing him to read that messy paper. What could delay a blindfolded substitute
> in just a few minutes?
> 
> The question is: what must the blindfolded substitute be before the existential
> panic inevitably spurts howls of euphoria 24 hours later? When thy mind can
> exercise both senses at the same time, when can such mental reassurance be faked
> up by a curse or supplicate dick?
> 
> I remember being near a friend who worked at the ocean pulpit. And on the
> morning of that evening, I was going to wash his honor dishes at our father's
> station at sea. On the next few days, we would leave for a midsummer setting at
> sea.
> 
> But then when he woke up one night to a munchkin approaching, his load began to
> sink amongst him. "Don't worry brats, imphebs– do you even sense the faintest
> cough!" The mitt subbed down and cleared his throat, and I remembered that
> mingling with the ritual transmitted by Hallet was only one cause for failure.
> Plush to called would not faze the tiniest smirk
