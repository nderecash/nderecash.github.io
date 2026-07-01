---
layout: post
title: "48 Hours to Build a Game: What Global Game Jam Taught Me"
date: 2025-04-03
categories: [Making]
tags: [Game Dev, Godot, Global Game Jam, Gamedev]
read_time: 5
excerpt: "We had 48 hours, three people, one Godot project, and a theme nobody expected. Here's what we built and what broke."
---

I had been learning Godot for about three months when Global Game Jam 2025 came around. I knew enough to be dangerous — which is to say, enough to be overconfident about what we could build in 48 hours, and not enough to avoid the crashes.

Bubblift is the game we made. It's an environmental awareness puzzle game where you guide bubbles through ocean layers — clean bubbles rise naturally, polluted ones need help, and the deeper you go the more hostile the water chemistry. Simple mechanic, legible theme, shipped in 48 hours.

Here's how it went.

---

## The team

Three people. Me, a graphic design student, and a computer science student who had never used Godot but could write C# quickly. The composition matters: we had skills that didn't overlap much, which meant we covered more ground but also meant there was almost no redundancy. When one person got stuck, the whole thing slowed down.

If I was doing it again, I'd want at least two people with overlapping technical skills so you can unstick each other faster.

---

## The first six hours: the dangerous part

The first six hours of a jam are the most important and the most likely to go wrong. This is when you agree on the game — the mechanic, the scope, the vibe — and the decisions you make here echo for the next 42 hours.

We made one good decision and one bad one.

**Good**: we scoped aggressively. Our first instinct was a multi-level puzzle game with unlockable characters and a narrative. We cut it to one mechanic, no characters, three levels. This was the right call. By hour 36 we were glad we had.

**Bad**: we spent two hours on art direction before we had a working prototype. The visual language of the game was decided before we knew if the core mechanic was fun. When the mechanic turned out to need adjustment — the physics felt wrong at the bubble density we'd planned — the visual decisions were already entangled with it.

Prototype first. Always.

---

## The middle: the actual building

Hours 6-36 were the real work. The mechanic is simple in concept: bubbles have properties (clean, polluted, heavy, light), the ocean has layers with different physics, and you apply force to bubbles to route them to the surface. The Godot physics engine handles most of this naturally, which saved us.

What didn't save us was scope creep in small pieces. A particle effect here. A sound effect there. A slightly more complex collision shape. None of these were wrong individually; collectively they pushed us toward hour 40 before we had a complete, playable loop.

The lesson: if you're adding something that will take more than 30 minutes, cut it. The game doesn't need it. You need the sleep.

---

## The last 12 hours: the scramble

Hour 36 to hour 48 was not fun. This is the part that people who describe game jams as "magical creative experiences" are maybe not fully remembering.

We had a working game. It was not polished. The sound design was incomplete. The tutorial didn't exist. The title screen was a placeholder. We had 12 hours.

We finished with 45 minutes to spare. The tutorial existed but wasn't good. The sound design was minimal but present. The title screen was no longer a placeholder.

I submitted and went to sleep.

---

## What Bubblift taught me about game design

A few things I took away:

**The mechanic has to be intrinsically interesting.** Bubblift works because the physics of bubbles is naturally satisfying — they wobble, they resist, they cluster. If your core mechanic isn't interesting to play before you add any game structure, the structure won't save it.

**Accessibility in games isn't an afterthought.** We didn't design Bubblift with accessibility in mind, and looking back at it through the lens of the research I was doing for Over the Barriers, there are things I'd do differently — clearer visual contrast, adjustable game speed, better colour-coding that isn't just hue-based.

**Shipping is the skill.** Making something complete, in the time you have, with what you know — that's the hard part. The technical skills you can look up. The decision-making under time pressure, the willingness to cut things, the discipline to say "this is done" — that's what jams teach you.

I'm doing it again next year.
