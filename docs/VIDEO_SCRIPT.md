# AI Employee Silver — Video Script

---

## OPENING  (0:00 – 0:20)

"What if you could hire an employee who never sleeps, never misses an email, posts on LinkedIn at exactly the right time, and always asks for your approval before doing anything important?

That's AI Employee Silver."

---

## PROBLEM  (0:20 – 0:45)

"Every business owner spends hours every week on repetitive tasks —
reading emails, replying to clients, drafting social media posts, following up.

These tasks don't need creativity. They need consistency.
And consistency is exactly what AI is good at."

---

## SOLUTION  (0:45 – 1:15)

"AI Employee Silver is an autonomous assistant built with Python and Claude AI.

It runs 24/7 in the background on your computer.
It monitors your Gmail — reads, classifies, and drafts replies automatically.
It manages your LinkedIn — takes a brief, writes a post, and waits for your approval.
And it can schedule posts for exactly the right time — like 9 AM tomorrow morning.

All of this happens without you touching anything."

---

## DEMO WALKTHROUGH  (1:15 – 2:30)

### Part 1 — Watchers Running
"Here you can see the system is already running.
Three watchers — Main, Gmail, and LinkedIn — all active with their process IDs."

### Part 2 — LinkedIn Brief Drop
"I drop a brief file into the intake folder.
Just a topic, tone, audience, and key points.
The LinkedIn watcher picks it up within seconds."

### Part 3 — Claude Drafts the Post
"Claude AI reads the brief and writes a full LinkedIn post —
professional tone, hashtags, call to action — everything ready."

### Part 4 — Approval UI
"Now I open the Approval UI at localhost:5050.
Here is the post, ready for review.
I can approve it for immediate posting —
or I can schedule it.
I type 09:00 — and the system schedules it for tomorrow morning at 9 AM."

### Part 5 — Scheduled Section
"The post now appears in the Scheduled section.
Look at the filename — it tells me exactly what it is and when it posts:
linkedin_2026-04-02_09-00_ai_automation_business.json

Tomorrow at 9 AM, the watcher will automatically move it to Approved
and post it to LinkedIn — without me doing anything."

### Part 6 — Gmail
"On the Gmail side, incoming emails are classified —
urgent, informational, client reply needed.
Drafts are generated and sent to the same approval queue."

---

## ARCHITECTURE  (2:30 – 2:55)

"The system has four layers:

Perception — watchers monitoring Gmail and LinkedIn continuously.
Reasoning — Claude AI classifying, drafting, and planning.
Scheduling — a dedicated Scheduled folder where approved posts wait for their time.
Action — approvers that execute only after human sign-off.

Nothing is posted, sent, or executed without the owner's approval.
Human-in-the-loop is not optional — it is built into the architecture."

---

## TECH STACK  (2:55 – 3:10)

"Built with:
- Python 3.14
- Claude AI — Haiku for fast tasks, Sonnet for complex reasoning
- Gmail API and LinkedIn API with full OAuth2
- Flask for the approval web interface
- File-based vault — every action is logged, nothing is silent
- Windows Task Scheduler for auto-start on login"

---

## CLOSING  (3:10 – 3:30)

"AI Employee Silver is not just a demo.
It is a working system that runs daily, posts real content, and manages real emails.

The goal was simple — give a business owner 10x output without 10x work.

Thank you."

---

## TIPS FOR RECORDING

- Screen record the terminal showing watchers running
- Show the Approval UI live at localhost:5050
- Show a post moving from Pending → Scheduled with a time set
- Show the Scheduled section with the filename format
- Keep background clean — VS Code or plain desktop
- Speak slowly and clearly — let the demo breathe
