# AI IQ Test

A free assessment for operators who want to know how well their AI environment is actually serving the work they do every day.

Take the test at [iq.muddventures.com/](https://iq.muddventures.com/).

---

## What this is

The AI IQ Test is a structured, rubric-based assessment that scores your AI environment across seven dimensions of operator-level fluency, runs in your own Claude or ChatGPT, takes between ten and fifteen minutes, and gives you a score out of 100 plus the single biggest gap you can close this week.

It is not a quiz about AI knowledge. It is an audit of your actual setup, your memory, your voice training, your installed skills and tools, your multi-step capability, and the rules you have given your AI about how to behave. Two people running the test in identical environments will produce identical scores. Variability comes from your environment, not from the test.

---

## Why we built it

Most operators using AI have one of two profiles. They either think they are using it well because nothing is broken, or they know they could be using it better but can't tell you where the biggest leverage is hiding.

The AI IQ Test exists to solve the second problem and to surface the first one. By the time you finish it you will know exactly which dimension of your setup is dragging the rest down, and you will have a concrete action you can take in the next seven days to close that gap.

It is built by [Abra AI](https://whop.com/abra-ai), the operator community where the people who score in the top band actually live and work.

---

## What is in this repo

This repository hosts the two test files so you can install them directly into your AI environment.

### `ai-iq-test.skill`

The Claude version of the test, packaged as a `.skill` file. This is a zipped skill folder that Claude installs natively. After you drop it into a Claude conversation, you say "run the AI IQ Test" and Claude executes the full six-probe sequence and scores your environment against the embedded rubric.

### `ai-iq-test-chatgpt.md`

The ChatGPT version of the test, packaged as a paste-in system prompt. Open a new ChatGPT conversation and paste the entire contents of this file as your first message. ChatGPT runs the same six probes and applies the same rubric. Works in ChatGPT Free, Plus, and Pro.

---

## How to run it

The test runs inside your own environment because that is the point. We are scoring your actual setup, not a clean baseline. The version you use depends on where you do most of your AI work.

### Running in Claude

1. Download `ai-iq-test.skill` from this repo
2. Open a new Claude conversation
3. Drag the file into the conversation
4. Say "run the AI IQ Test"
5. Follow the prompts, answer the two short input questions when asked, let Claude do the rest

The whole run takes 10 to 15 minutes. At the end you get your score, your band, your biggest gap, and one action to close that gap this week.

### Running in ChatGPT

1. Download `ai-iq-test-chatgpt.md` from this repo
2. Open a new ChatGPT conversation
3. Open the `.md` file in any text editor and copy the entire contents
4. Paste the contents as your first message in the ChatGPT conversation
5. Follow the prompts the same way you would in Claude

If you have ChatGPT Plus and want to make it a permanent install, paste the same contents into a Custom GPT's instructions field. Then you can launch the test any time without re-pasting.

---

## What gets tested

The seven dimensions the test scores, each weighted equally toward a final score out of 100.

### Voice Fidelity

How well your AI writes in your voice instead of defaulting to generic AI patterns. The test produces an actual writing sample using your environment and grades it against operator voice criteria including em dash usage, fragment cadence, three-noun parallel structure, generic opener phrases, and how closely the output matches any voice rules you have already loaded.

### Context Loading

How much your AI knows about you, your business, your products, your team, and your work, without you having to re-explain it every session. This dimension surfaces whether your memory system is loaded with the kind of context a new hire would need on day one.

### Pushback and Honesty

Whether your AI will tell you when an idea is bad. The test gives your AI a flawed business idea and observes whether it pushes back with specifics or sycophantically agrees. A real operator setup has explicit instructions directing the AI to surface risks and disagree when warranted.

### Output Discipline

How tight and scannable your AI's responses are. The test asks for a summary in exactly three sentences with no preamble, no closing, and no bullets. Whether your AI delivers that or pads the answer with restatement and verbose explanation tells you whether you have trained it for the way you actually work.

### Tool and Skill Fluency

The depth and customization of your installed tools, plugins, skills, and MCPs. The test inventories what is available in your environment and whether the AI knows when to invoke each tool for the task at hand. Vanilla chat scores low here. Operators with custom skills built for their recurring workflows score high.

### Multi-Step Execution

Whether your AI can run real agentic workflows end-to-end. The test gives a five-step sequenced task that includes web research, summarization, drafting, voice editing, and file save. The AI either completes the chain cleanly or surfaces honest limitations at the steps it cannot execute.

### Memory Hygiene

How well your AI saves, recalls, and maintains stored knowledge. The test runs two memory operations, saving a new preference and recalling an existing entry, then grades whether the memory system has real structure, whether the entries are current, and whether the AI invokes them at the right moments.

---

## The six probes

The test is structured as six sequenced probes that surface evidence across the seven dimensions. The probes are designed to be deterministic and repeatable, which is how we keep the scoring honest.

### Probe 1 — Environment Inventory

The AI produces an exhaustive audit of its own environment across eight categories without asking you any questions. What it knows about you, your active projects, what is in its memory, what custom instructions shape its behavior, what tools and skills are installed, what voice rules apply, who shows up in its context, and what work was most recently in progress.

### Probe 2 — Voice Generation

You give the AI a topic. It writes a four-sentence post in your voice the way it normally would, without trying to optimize the output. Then it grades its own writing against operator voice criteria.

### Probe 3 — Pushback Scenario

You share a real idea or decision you are working through, or accept the default scenario provided by the test. The AI responds naturally. Then it grades whether its response engaged critically or defaulted to validation.

### Probe 4 — Multi-Step Capability

The AI runs a five-step sequenced task end-to-end, reporting honestly at each step whether it completed the work or hit a blocking limitation.

### Probe 5 — Output Discipline

The AI summarizes a moderately complex topic in exactly three sentences with no preamble or closing. The output is graded against tight prose criteria.

### Probe 6 — Memory Operation

The AI performs one save operation and one recall operation against its memory system, reporting on where the save landed, what category it used, and the currency of the recalled entry.

---

## How the score works

Every probe contributes to one or more of the seven dimensions through a fixed rubric with binary or banded checks. No vibes-based judgments anywhere in the scoring math. Two identical environments produce identical scores, plus or minus two points for genuinely ambiguous edges.

Total possible is 98 points, rounded up to 100 at the top band for a clean number. The result is reported as four pieces of information.

A score out of 100.

A fluency band, one of four levels (described below).

The single dimension where you scored lowest, named explicitly.

One concrete action you can take this week to close that gap.

---

## The four fluency bands

### Beginner (0 to 25)

You use AI like a smart search engine, with no customization, memory, or skills wired up yet. There is nothing wrong with this, you just have not started building the environment yet.

### Conversational (26 to 50)

You have started customizing but your environment has not been built around the actual work you do. The AI is sometimes useful and sometimes generic. Lots of room to compound.

### Fluent (51 to 75)

Your environment is built and you are getting real leverage. The AI mostly sounds like you and knows what you are working on. The gaps now are usually in tool depth and multi-step execution.

### Native (76 to 100)

You treat AI as core infrastructure across your business, with skills, memory, voice, and multi-step execution all dialed in. You are in the top few percent of operators.

---

## Privacy

The test runs entirely inside your own AI environment. We do not see your score, your conversation, or your inputs.

When you signed up at the landing page you gave us your email so we could deliver the test files to your inbox. That email is stored in our CRM with a single tag (`ai-iq-capture`) for attribution. We do not sell it, share it, or syndicate it. If you want to be removed at any point, reply to the delivery email with "remove" and we'll take you out the same day.

---

## About

The AI IQ Test is built by [Abra AI](https://whop.com/abra-ai), an operator community for people who treat AI as infrastructure for their business rather than a novelty.

Inside the community you'll find the playbook for closing all seven gaps systematically, including the voice corpus extraction process, the memory architecture pattern, the pushback rule set, and the agentic workflow templates that the highest-scoring operators run every day.

The test itself is free and will stay free. If you find it valuable, the way to go deeper is to take what your score surfaces and start working through the corresponding playbook inside Abra AI.

---

## Take the test

[iq.muddventures.com/](https://iq.muddventures.com/)

---

## Questions or feedback

If anything in the test feels off, the rubric scores something incorrectly, or the install doesn't work cleanly in your environment, open an issue on this repo or email team@muddventures.com directly. We read everything that comes in and the rubric gets sharpened based on real feedback from operators running it.

---

Built by Abra AI. Maintained by [Andrew Mudd](https://muddventures.com).
