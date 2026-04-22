# Your Apprentice Is Your Biggest Security Hole

_**Information Security** · Rainmoon 21_

> **TL;DR** Your apprentice is not a traitor. Your apprentice is twenty years old, talks to people their own age, and has never had anything worth stealing. They're not going to keep your secrets safe by accident. They need a threat model, training, and a set of rules simple enough to follow at a tavern.

I'm going to make a confident prediction. If your sanctum is breached in the next year, it will not be breached by a rival archmage, a demon, or a particularly clever dragon. It will be breached because your apprentice mentioned the location of something, in passing, at a wedding.

I'm not being cruel. I was twenty once. I talked about things I shouldn't have, at weddings and otherwise. The only reason nothing bad came of it is that I wasn't working for anyone important. Your apprentice is working for you. That's the difference.

## The apprentice threat profile

Let me describe your apprentice's security posture as we usually find it, when we do an infosec audit. I'm composing from twenty years of notes; no single real apprentice is this bad, but the composite is instructive:

- Shares a bedchamber at the academy with three other apprentices, one of whom is the cousin of a local thief.
- Keeps a journal. Not warded. Under their pillow. Contains at least four details about your sanctum.
- Has a sweetheart in the next village who is, statistically, somebody's informant. (Not through malice. Villages are small. Every sweetheart is somebody's informant.)[^1]
- Has, at some point in the last six months, complained about you in a tavern.
- Believes, in their heart of hearts, that security is your problem, not theirs.

None of this makes them a bad apprentice. Some of it makes them a normal human. All of it makes them a vulnerability.

## Why the standard advice doesn't work

The standard advice is: "Don't tell your apprentice the important things."

This is bad advice for two reasons. First, you have to tell them _some_ things, or they can't function as an apprentice. Second, and more important, it's an adversarial framing. It teaches the apprentice that the master doesn't trust them, which makes them less careful, not more. If you're already assumed to be leaking, why bother plugging the leaks?

The correct framing is: **teach them to be part of the defense.** Give them a threat model. Give them rules. Make it their problem too.

## The rules we give apprentices

This is from our standard half-day training. We call it "What To Say At The Tavern." It has five rules.

### Rule 1: Never name the location of a component or a book.

Not the room. Not the shelf. Not "the north wing." Apprentices love to drop that they know where things are, because it makes them feel important. Nothing you say about the location of anything valuable in your master's sanctum is safe. If asked: "I'm not sure, honestly. The master moves things." This is a good answer. It doesn't even have to be true.

### Rule 2: Never confirm what you're researching.

If someone you don't know asks what you've been working on, the answer is always "boring stuff, mostly copying." Real research is never discussed with strangers. Real research is barely discussed with friends. This includes sweethearts, in case that wasn't obvious.[^2]

### Rule 3: Never confirm the master's schedule.

"When does he leave the tower?" "I don't know, honestly, he keeps his own hours." "When does he sleep?" "I've never noticed." Even if you _have_ noticed. Schedule information is the single most valuable thing an apprentice knows. Protect it like you'd protect your own pay.

### Rule 4: If someone is asking strangely specific questions, leave.

You don't have to be clever. You don't have to catch them out. You just leave. Go to the privy. Don't come back. We would rather you be rude than be a source.

### Rule 5: Report the conversation to the master the next day.

Every single time. Even if it was nothing. _Especially_ if it was nothing, because small probes are how bigger cons start. The master is not going to yell at you for reporting nothing. The master is going to yell at you for reporting nothing four months after the break-in, when you suddenly remember.

## What the master has to do

The other half of this, and the part wizards resist: you have to make it safe for the apprentice to report.

If you yell at them for reporting a false alarm, they will stop reporting. If you mock them for being careful, they will stop being careful. If you punish them for the inevitable mistake, they will hide the next mistake.[^3]

The master's job is to receive every report calmly, say "thank you for telling me," and move on. This is harder than it sounds. It is also the single most leveraged thing you can do for your security.

## The inconvenient summary

Your apprentice is a hole in your security. You cannot plug the hole by firing them or mistrusting them. You plug it by training them, giving them rules simple enough to remember when drunk, and making it safe to report mistakes.

We do the training. It takes half a day. We've been told by one wizard — not Archibald this time — that it was the best investment he ever made. He said so in a very dry tone. That's the highest praise a wizard will ever give anything.

[^1]: We have literally never audited an apprentice whose sweetheart, in retrospect, was not also feeding information back to _someone._ Not always a bad someone. Just someone.

[^2]: It is never obvious. We add this to the training explicitly because apprentices read the first four rules and then go tell their sweetheart all five rules that evening.

[^3]: The apprentice who hides mistakes is how you lose a tower. The apprentice who reports their mistakes immediately is how you keep one. Train the right one.
