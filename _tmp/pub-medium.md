# The AI Coding Speed Illusion: Why Experienced Developers Got 19% Slower

I code with AI almost every day, and every time, it feels faster. Code fills the screen in seconds, and a function I've been stuck on for an hour suddenly works. So when I first read the results from METR, a research group that studies AI capabilities, I felt a jolt. They handed AI tools to experienced developers and measured a 19 percent *increase* in the time it took to finish tasks. The stranger part: those same developers walked away convinced AI had made them 20 percent faster.

## What the Study Actually Found: Gut Feeling vs. the Stopwatch

In early 2025, METR recruited 16 experienced open-source developers, people with an average of five-plus years working on their own codebases, and had them tackle 246 real coding issues. Each task was randomly assigned to either an AI-allowed or AI-forbidden condition, and completion time was logged ([METR](https://metr.org/blog/2025-07-10-early-2025-ai-experienced-os-dev-study/)). Their tools of choice were Cursor Pro and Claude 3.5/3.7 Sonnet.

The numbers tell a strange story. Before the study started, developers predicted AI would cut their time by 24 percent. The actual result was a 19 percent increase (95% CI: +2% to +39%). Here's the part worth sitting with: even after the study ended, having just lived through the slowdown themselves, developers still estimated that AI had sped them up by 20 percent ([arXiv](https://arxiv.org/abs/2507.09089)). What they felt and what the clock recorded pointed in opposite directions.

## Why the Illusion of Speed: A Cognitive Debt Lens

There's a concept I'd written about in my notes a while back that explains this gap: cognitive debt. In AI-assisted development, the speed at which code gets produced routinely outpaces the speed at which I actually understand it.

![Diagram showing how code-production speed outpaces comprehension speed, creating a cognitive-debt gap](https://cdn.jsdelivr.net/gh/jalnanco/notemad-blog-photos@main/published/ai-coding-productivity-illusion-metr/cognitive-debt.png)

That's where the illusion takes hold. Finished code piles up in front of you, so the work looks like it's moving. But if you never fully absorb why the code was written that way, or where it might break, that unpaid balance doesn't disappear. It gets billed later. It shows up when a reviewer flags something you can't explain, when you're stuck untangling an edge case, or when you need to roll back a change and don't know which parts to undo. Production is visible, so it registers as fast. The gap in understanding shows up later, as time, which is why the slowdown is so easy to miss.

## Should We Ditch AI Coding? It Comes Down to How You Use It

Jumping to conclusions here would be a mistake. The study comes with caveats: early-2025 model capability, mature codebases with five-plus years of history, and experienced developers. The better you know your own codebase, the more likely it is that explaining context to the AI and checking its output costs more time than writing the code yourself would have.

METR didn't treat this as the final word, either. In a follow-up, they scaled the study to 57 developers and roughly 800 tasks, and ran into selection bias. Developers who felt they "couldn't work without AI" dropped out of the study, and 30 to 50 percent of participants held back tasks they expected AI to help with most. So the team is redesigning the experiment: fixed tasks the developers don't get to pick, AI use randomized at the developer level, and real usage logs from tools like Claude Code folded in as observational data ([METR](https://metr.org/blog/2026-02-24-uplift-update/)). The real question is shifting from whether AI is good or bad to how you actually operate it.

## My Three-Question Check Against the Speed Illusion

Before I hand off code I wrote with AI, I ask myself three questions. Can I explain the core logic and error handling of this change to someone else in five minutes? Can I write down, in a couple of lines, why I chose this approach over another? Do I know exactly what to roll back if this fails? If I get stuck on any one of them, I treat that feeling of "this went fast" as the sound of cognitive debt piling up.

I'm not giving up AI. I've just stopped trusting the feeling of speed on its own. Speed gets measured with a clock; understanding gets checked by explaining it out loud. METR's 19 percent doesn't mean stop using AI. It means your own sense of how fast you're going deserves a second look.

Thanks for reading, cheers.
