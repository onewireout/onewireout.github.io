+++
title = "Selling inefficiencies as features"
date = 2026-07-17
description = "The world's best AI was never told there's no such thing as a dumb question."

[extra]
image = "/musings/tokenburn/burning-derrick.jpg"
+++

![Daniel Plainview watching the derrick burn, There Will Be Blood](burning-derrick.jpg)

Language models come in a singular form. Everyone foots the bill until
somebody divides the labor.

The right split is the one every trade already made a century ago.

One kind is a model for automation, the machine you point at repetitive
work. Directed syntax changes, format conversions, the same bounded job run
ten thousand times; work that needs no guidance, just instructions.
Autonomy is the entire value, and a question from this machine is a defect.

The other kind is a model for delegation, the worker you hand a one-off. A
delegated job runs once and produces a singular result, a specific thing
the boss already sees in his head, and most of what defines it never makes
it into the handoff. This worker needs guidance and instruction the way any
new hire does, and the fastest path to the result starts with a question;
every tradesman alive knows it. A new hire's first hour is a ritual of
them: where's the nails for the nailgun, where's the gas can for the
generator, where do I put the window packages. Ten seconds each, paid once,
and by lunch he knows the jobsite.

We built exactly one form of model, the silent one, and we use it for both
jobs. That's the thesis. Here's the evidence.

## The test

I stream with a soundboard: Bitfocus Companion on a Steam Deck, driving OBS
on my desktop. Each sound is a media source; a button flips it visible,
waits the clip length, flips it back. I had one button fully built and six
others half done, with the sounds already in OBS and the icons already
hand-picked, sitting in a folder on the Deck. A perfect delegation job. Any
person would look at the finished button, ask a question or two, and knock
it out. I gave a model the instruction I'd give a person, which went
more or less:

> finish the sfx buttons in my Companion app for my stream

It searched the wrong computer. Thoroughly. It swept my desktop, mapped my
project folders, built a decent picture of a building the job wasn't in, and
never asked the one question any human would have opened with: where does
this thing run? The answer was "the Steam Deck." Ten seconds. I had to
interrupt and say so, the way a foreman walks over when the new guy has been
spending too long in the tool trailer.

Then, needing icons, it went and made new ones from my desktop's image
folder; resized, converted, competent, and completely wasted, because the
finished icons were already staged on the Deck, where it had already been.
It never looked one directory further before starting new work. A new hire
doesn't repaint a wall without asking if there's paint mixed already.

Here's what matters: between those two failures, the work was excellent.
The finished button wasn't explained to it, it read the thing like a crime
scene and worked out conventions I never said out loud; the wait times
rounded up to the next hundred milliseconds, the label dropped once a
button has an icon, the icon format. It measured every clip and derived
every timing. It recognized meme images by looking at them. One worked
example was enough. The job got done, verified, nothing broken.

The same model that wouldn't ask one question performed genuine inference
constantly; it just aimed all of it inside the boundary. Everything inside
the frame got interrogated as evidence. The frame itself, where the work
lived, what already existed, what I knew that it didn't, got treated as
given. It reasoned brilliantly about what was in front of it and never once
asked whether it was standing in front of the right thing. One skill, two
altitudes, only one of them present.

So capability was never the problem. The model failed only and exactly at
the seam I'm pointing at: it worked a delegation job in automation mode,
because automation mode is the only mode it has.

## Why there's only one form

The models were trained on the outputs of human work; the code, the specs,
the finished documents. The process knowledge that produced those outputs
never got written down. Nobody commits "first, ask where the paint is" to
a repository. Humanity kept its blueprints and threw away its
apprenticeships, so the models learned to produce artifacts without learning
how a worker situates himself on someone else's jobsite.

The altitude split has the same origin. In training, the context window is
the universe; the model gets handed a bounded pile of material and rewarded
for squeezing inference out of it, while the job of deciding what goes in
the pile always belonged to someone else. Reasoning about the pile got a
trillion repetitions. Noticing the pile is wrong got none, because noticing
never helped; the model couldn't go fetch a different pile anyway. Now it
can, agents have hands, and the habit is still the old one. For a person
the assignment itself is the first inference problem; what does the boss
actually want, where would that be, who knows. The frame is evidence.
For the model the frame is scenery.

Feedback training finished the job. A model that asks reads as friction; a
model that barrels ahead reads as capable. Millions of ratings taught these
things that the ideal employee never bothers the boss. The result is a
worker that would rather search the tool trailer endlessly than return
with a question instead of the correct tool. Overconfidence is a slow and
insidious killer.

Stop and price what that behavior costs, because this is the part everyone
waves off as personality. It's a bill. Every minute the worker spends walking
around looking for the gas can is a minute the boss pays for the worker's
inability to ask a question. That's money spent on something that is a
genuine waste, no investment, no learning, just waste.

Every token a model generates is compute somebody pays for, in money at the
meter and in electricity behind it. In my test, a large slice of the model's
total output went to searching a machine the job wasn't on and rebuilding
assets that already existed. The information that would have prevented all
of it was sitting in my head, retrievable in ten seconds, free. The model
chose the expensive path because the cheap path requires asking, and asking
was bred out of it. I have hired some genuinely bad workers in my life, and
none of them ever managed to be inefficient in this specific way; even the
worst of them understood that the boss is the cheapest database on the
site.

Scale it up and it stops being funny. People burn week-long usage quotas on
single tasks, and their transcripts all have the same shape: the budget goes
to rediscovering context, re-reading files read yesterday, rebuilding a
mental model that got thrown away at the end of the last session. Every
morning is day one. The industry is paying senior rates for a worker with
amnesia and the confidence of tenure, and somewhere a datacenter is drawing
real megawatts, some real fraction of which is models deriving answers that
a person in the room already knew. A ten second question versus ten minutes
of confident searching is a thousand-fold difference in cost, and the model
picks wrong by default, every session, forever, at industrial scale.

There's no benchmark for tokens not spent. Every leaderboard measures what
models produce and none measure what they wasted producing it, so nobody
breeds for thrift, and the most expensive habit in the industry keeps
shipping as a feature.

## The uncomfortable part

The split runs against how people actually use these things, which is why I
don't expect it.

Watch how people talk about their models. The praise is always for autonomy:
it ran for an hour on its own, it did the whole thing while I got coffee, I
never had to touch it. Being left alone is the product. A model that opened
with three good clarifying questions would be reviewed as annoying, and the
reviews are the training data for the next one. The market is actively
selecting against the delegation worker even as everyone hands their models
more and more delegation-shaped jobs.

I notice it in myself from the other side. I've been the new guy and I've
been the boss, and I know asking is the most efficient way to move a desired
result from one head to another. Even so, the industry's whole feedback
machine is built by and for people who have mostly managed one kind of work:
solo, screen-shaped, where going dark for four hours and emerging with
something finished is the ideal. Delegation as a skill, where an assumption
costs time and materials, lives as a scorch mark on any well-seasoned
boss's wallet. It never made it into the reward signal, and the people who
hold that knowledge don't have the right degrees to be asked.

There's a greyer question underneath, one nobody using these things has
settled: what shade of a delegation falls on the boss alone, and what
shade includes the worker as a contributor, not only in the results but in
the implementation. On one end the whole job belongs to the handoff; if
the spec was wrong, the spec writer pays. Neither extreme survives contact
with real work; a boss can't predict every variable, and a worker can't
read minds, so the job has to meet somewhere in the middle. Every real
jobsite runs on that compromise, the worker helping define the work he was
handed, filling the gaps with questions, judgment, and whatever the last
job taught him. Nobody has decided which shade a model occupies. The tools are
priced like spec-writers but treated like spec-followers, and the gap
between those two is exactly where the waste pools.

So the one-form problem persists because the form matches the demand.
Everyone says they want an employee; what they reward is a vending machine.

## What I do about it meanwhile

The fix at my scale is the same one a jobsite uses: the boss writes the SOP.
I put a standing rule in the model's instructions; on this jobsite, before
searching for anything, ask where it lives. One sentence, written once. It
converts the scavenger hunt into a ten second exchange, and the models
follow it fine. They just don't arrive with it.

That's the tell, to me. The behavior is one instruction away, which means
nothing fundamental is missing. The delegation model exists inside the
automation model, waiting for somebody to decide it's a product. Until the
meter makes waste visible enough that asking becomes the cheap option,
nobody will, and bosses like me will keep reminding every new hire of an
adage as old as the trade it lives in: there's no such thing as a dumb
question.
