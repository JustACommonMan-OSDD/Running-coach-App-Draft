# Kickoff meeting notes

Friday 2 October 2026, 29 minutes.  
Present: `Customer`; `@Ezekiel-Gadzama` (interviewer); `@Obetech1`; `@Sirjaey`; `@JustACommonMan-OSDD` (timekeeper).

What was said, in order. Timestamps are elapsed time from the start of the recording.

## Opening

**[00:26] `Customer`** confirmed the project is a coach app and asked whether the team had done prior research and how they wanted to proceed.

**[00:45] `@Ezekiel-Gadzama`** asked why the `Customer` put a coaching app forward, and what problem he believed it would solve.

## The `Customer`'s description of the product

**[01:24–07:17] `Customer`.** Running on its own is boring; someone encouraging you makes it better. He wants a voice that varies the intensity during the run — thirty seconds as hard as you can, then medium, then jog — and reads your stats back at intervals you set, say every three minutes: pace, distance, heart rate.

He has seen the idea in pieces. Zombie-chase running apps exist; he does not like the zombies, but the structure interests him. The model he gave was a knowledgeable friend who phones you, stays on the line while you run, encourages you at different intensities, and sends a summary afterwards.

He believes an LLM small enough to embed on the phone would be enough — he named Gemma from Google — with text to speech, and no server. Because the microphone is open, breathing could be counted and used as a signal. You could also talk back to it and ask questions mid-run.

He uses Google Health and dislikes it: there is a lot in it, but "it all requires me staring at stats on the phone, it doesn't talk to me." On a treadmill the machine tells you where you are; outdoors you have to pull the phone out.

He asked the team to start simple, with running only, and said the shape of the ten weeks can run from a basic app that follows you and reports distance, up to a conversational coach.

## Friend and social features

**[07:17] `@Ezekiel-Gadzama`** summarised the request back, then asked whether runners should be able to see a running partner's stats — heart rate, average speed — while running together.

**[08:10] `Customer`** said get the personal case working first. Sharing between accounts means connections, security, sharing and unsharing data, which is "a project on its own", and he doubted ten weeks would reach it. He left it open as a later paid tier if the team continues after the course.

## Health data

**[09:53] `@Ezekiel-Gadzama`** asked whether users should upload health or medical documents, so the app could warn them before, for example, a heart problem — and if so, in what format.

**[10:54] `Customer`** said start with whatever the phone gives: acceleration and other sensors. A wearable such as a watch would be good to get and worth exploring, but he was not sure it was reachable. Uploading documents comes much later, and in his experience people will not do it — they are either too lazy or treat it as a security problem. He added that the goal is not to collect data, it is to help people exercise, and that running was chosen because it is the easiest exercise to detect.

## Comparable products

**[13:42] `@Ezekiel-Gadzama`** asked whether the `Customer` knew an application closer to what he wants than Google Health.

**[14:05] `Customer`** said no. He has seen the functionality in bits and pieces — a YouTube track that talks you through a run with no interactivity, some paid apps — but nothing matching. He invited the team to research and propose something. He added that he would rather the data were processed on the phone than sent to the cloud.

## Goal setting

**[15:38] `@Obetech1`** asked whether the app should help a runner set a goal — a fitness target, or what to eat after a session.

**[16:19] `Customer`** said he has not seen goal setting done well. What works, in his experience with language-learning apps, is not asking the user for granular controls but offering preset milestones. Applied here: offer a small number of programmes rather than fine-grained configuration — simpler to build and probably what the user wants anyway.

He was explicit about the order: the base is the app talking to you and reporting how long you have run, your speed, heart rate and perhaps breathing rate, so you never look at the phone. A choice between two simple programmes comes on top of that, later, once there is user feedback.

## Language and distribution

**[20:00] `@Ezekiel-Gadzama`** asked which language the first version should be in. **`Customer`:** English — the team is comfortable with it, he is, and half the world is. Russian can follow later if someone wants it.

**[22:25] `@Ezekiel-Gadzama`** asked whether availability outside Russia should be designed for, given restrictions on external resources.

**[22:50] `Customer`** said the Android store works in Russia, and the app could also be open source on GitHub for anyone to download. He asked the team to target **Android, not iOS**, because he has no iOS device and could not test it.

He then stepped out of the customer role: the project is "just a vehicle for you to practise processes" in the course, so where it is published matters less than that it is published and the team can show proof. He added that he would still like it to reach as wide an audience as possible.

## Target user

**[23:28] `@Sirjaey`** asked whether to design for a complete beginner, for someone who can already run 5 km, or for anyone — whether there is a specific target runner.

**[23:55] `Customer`** said **beginner to intermediate**. Marathon runners may have specific requirements for their training regimen that he does not know. He saw no reason the product could not move toward advanced users later, and noted that even a marathon runner would want stats read out without looking at the phone — all of which needs is a headphone. He then asked the team whether any of them knew professional runners and what those runners need. No one answered.

## Close

**[25:52] `@Ezekiel-Gadzama`** thanked the `Customer`, said the team would go away and discuss the design, and would show him iterations.

**[26:20–29:08]** Scheduling. The next meeting was agreed for **Tuesday**. The `Customer` asked for **08:00 WAT** if possible — it was 21:30 where he was — and the team offered 08:30. Left to be settled offline. The `Customer` said he would send a note.

## Not covered

Three starred questions from [meeting-script.md](meeting-script.md) were not asked: Q3 (what a runner you know records their runs with), Q7 (what you did the last time an app changed a workout on you), and Q10 (which of the two propositions ships first). Q11, whether a rule-based engine is acceptable rather than machine learning, was also not asked, although the assumption table in [value-proposition.md](../../docs/research/value-proposition.md) lists the kickoff as where it would be checked.

The `Customer` did not mention training plans, race goals or plan changes at any point.
