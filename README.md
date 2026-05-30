# Haunt

"You're never as alone as you think"

The Core Philosophy
The app never once says "make friends" or "meet people." Every feature has a utility or curiosity disguise. Connection is always the side effect, never the stated goal. Three layers working together:
PULSE    →    the utility layer      (why you open it)
ECHOES   →    the discovery layer    (why you keep coming back)
SHADOW   →    the connection layer   (why you stay)

FEATURE 1: THE PULSE
"What's happening right now"
This is the front door of the app — what it looks like to the outside world. A campus map showing the live vibe of every location.
What you see:

A map of campus with locations glowing based on activity
Each spot has a vibe tag — "focused energy," "chaotic," "chill," "packed," "dead" — crowd-sourced passively from who's there
A busyness meter so you know if the library 4th floor has seats
Recent echoes teasing from each location ("3 new drops at Free Speech Café")
Live headcount — "14 people here right now"

Why it works:
Students open it the same way they'd check Google Maps for a restaurant wait time. Zero social intent. Pure utility. But the moment they open it, they're in the ecosystem.
Key mechanic — passive check-in:
You don't manually check in. The app detects you're at a location via geofence and quietly registers your presence. No action needed. This feeds into everything else.

FEATURE 2: ECHOES
"Leave a trace. Find one."
This is the geocaching layer. Digital messages, photos, and voice notes anchored to physical spots — invisible until you're standing there.
Dropping an Echo:

Arrive at a location → tap the drop button
Leave a text note, photo, short voice memo, or drawing
Choose: public (anyone who visits sees it) or whisper (only your Shadow match sees it)
Set a lifespan: 1 hour / 24 hours / 1 week / permanent
Optional mood tag: funny / honest / observation / rant / wholesome

Finding an Echo:

Walk to a location → Echoes from that spot materialize on your screen
Older or rarer Echoes are more buried — you "dig" by visiting repeatedly
You can react but not reply publicly — reactions are anonymous
Some Echoes are layered — a note left months ago that's still there, buried under newer ones

Example Echoes in the wild:

"the 4th floor bathroom mirror has excellent lighting. use it." — Free Speech Café, 3 days ago


"I've cried in this stairwell twice. it's a good stairwell." — Soda Hall, 2 weeks ago


"whoever is always here at 2am — you're not alone" — Moffitt Library, 1 month ago

Why it works:
It turns every campus spot into a living scrapbook. Students explore locations specifically to find Echoes. The curiosity loop is completely separate from any social pressure.

FEATURE 3: THE ROOM
"The group chat for wherever you are right now"
This is the hyper-local anonymous chatroom. Every physical location has one. You're in it automatically when you arrive. You leave it when you go.
How it works:

Enter a geofenced location → you're silently dropped into that location's Room
See only messages from people physically present right now
Completely anonymous — you're just a random color and shape ("Blue Triangle," "Orange Circle")
Chat disappears when you leave. No history. No receipts.
Messages older than 30 minutes fade out even mid-session

What it naturally becomes:
"ok who is stress-eating chips loudly rn 😭"
"LMAO that's me I'm so sorry"
"honestly same energy"
"does anyone actually understand this problem set"
"no but I've been staring at it for 2 hours"
"want to just suffer together"
Moderation mechanic:
Since everyone is physically present, toxicity is naturally suppressed — you're talking to someone in the same room. But there's also a tap-to-flag system: if 3 people flag a message it disappears instantly, no questions asked.
Persistence bridge:
If two people have been in the same Room together 3+ times across different sessions, the app quietly takes note. This feeds directly into Shadow matching.

FEATURE 4: SHADOW
"Someone haunts the same spots as you"
This is the invisible pen pal layer. The app watches where you go, when you go, and how long you stay — and finds your ghost.
How matching works:
You study at Moffitt 4th floor every Tuesday/Thursday night
Someone else does the same
You've been in the same Room together without knowing it
Overlap threshold hit → Shadow match unlocks
The match notification:
Not "You have a new match!" — instead:

"A ghost haunts the same spots as you. They left you something."

The Shadow chat:

Fully anonymous — no names, no photos
Anchored to your shared location ("your corner of Moffitt")
Conversation starters are auto-generated from your shared context:

"You're both always here on Thursday nights"
"You've both dropped Echoes at this spot"
"You were both in the Room here last Tuesday at midnight"


No swiping, no profile-browsing — just two people who already share something talking about it

The slow reveal:
Shadow chats have a natural escalation arc built in:
Week 1: Anonymous, location-anchored small talk
Week 2: Interests start slipping through naturally
Week 3: You know their vibe, their humor, their schedule
Week 4: App gently prompts — "your shadow is here right now"
         → you decide if you want to find each other
         → or stay shadows forever. both are valid.
The meeting is always optional. Some people will stay pen pals for a semester and never meet. That's a feature, not a bug.

FEATURE 5: CONSTELLATIONS
"Your people, without knowing they're your people"
Over time the app builds a private map of your campus life — not shared with anyone, just yours.
What it tracks:

Your most frequented spots and when
Echoes you've dropped and their reactions
Rooms you've been in and the general vibe
Your Shadow match history (anonymized)

What it shows you:

"You spend most of your time at 3 spots. 47 other people do the same."


"Your Echo at the Campanile has been found 12 times"


"You've been in the same Room as the same anonymous person 6 times this month"

It reframes loneliness statistically — you are not isolated, you are overlapping with dozens of people constantly and just never knew it.

THE FULL ARCHITECTURE
┌─────────────────────────────────────┐
│              THE PULSE              │
│     Campus map. Vibe. Busyness.     │
│        The reason you open it       │
└────────────────┬────────────────────┘
                 │
     ┌───────────┴───────────┐
     ▼                       ▼
┌─────────┐           ┌─────────────┐
│  ECHOES │           │   THE ROOM  │
│ Leave & │           │ Live anon   │
│ find    │           │ location    │
│ location│           │ chatroom    │
│ messages│           │             │
└────┬────┘           └──────┬──────┘
     │                       │
     └───────────┬───────────┘
                 ▼
         ┌──────────────┐
         │    SHADOW    │
         │ Passive pen  │
         │ pal matching │
         │ from overlap │
         └──────┬───────┘
                ▼
        ┌───────────────┐
        │ CONSTELLATIONS│
        │  Your private │
        │  campus life  │
        │  map          │
        └───────────────┘

WHAT MAKES THIS DIFFERENT
Every other campus appHauntYou sign up to be socialYou just exist on campusProfiles and photosColors and shapesOpt in to connectConnection finds youCampus-wide feed gets toxicRoom resets, presence = accountabilityForces the friendshipFriendship is always optionalFull anonymity = crueltyPhysical presence = natural civility

BUILD ORDER
If this were a real product, what to build first:
V1 — Prove the concept:
The Room only. One building, one university. See if the organic chat behavior happens naturally.
V2 — Add the hook:
Echoes. Now people have a reason to physically explore campus. Retention goes up.
V3 — Add the magic:
Shadow matching. This is the feature that makes people tell their friends about it.
V4 — Add the depth:
Constellations. The feature that makes people feel seen by their own campus.
