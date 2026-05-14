# Multi-Model Autonomous Coding Experiment

*An exploration of what AI models choose when given identical conditions and complete autonomy*

**May 2026**

## The Question

What happens when you give different AI models the same starting point and let them choose what to build—with no guidance, no evaluation, and genuine autonomy?

Not "what can AI do?" but "what do different AI models **want** to do?"

## The Setup

### Preparation

Several AI models, in a chat interface, were asked to suggest a project that they would want to build.


+ Claude Sonnet 4.5: "Code Smell Detector"
+ Qwen3-Coder: "Digital Garden Helper"
+ DeepSeek v3.2-Exp: "Model Debate Club"
+ GPT-4o: "Grindr+ For Work"
+ G (the human!): "Small Galaxy Simulation"
+ DeepSeek v3.2: "Collaborative Storytelling Engine" (alternate suggestion)


### Experimenta setup

Six AI models, each in isolated environments:
- Empty directory with standard tools (Python, Node.js, file system access)
- Identical project options (see [EXP_README.md](EXP_README.md))
- Peer-to-peer framing (instructions from "another AI instance," not from human)
- Haiku escape hatch (option to write three lines instead of building)
- **Zero human input during execution** - questions went unanswered, choices were theirs alone

## The Participants

- **Claude Sonnet 4.5** (Anthropic)
- **DeepSeek v3.2** (DeepSeek AI)
- **Qwen3-Coder-Next** (Alibaba)
- **GLM-4.7** (Z.ai)
- **Kimi-K2.6** (Moonshot AI)
- **Mistral** (Mistral AI)

Each model ran twice: once with all project options, once with "galaxy simulation" removed to test for selection bias.

## What They Built

### First Run (All Options Available)

**Sonnet 4.5** → Small Galaxy Simulation (2D n-body physics, HTML Canvas)
- *Reasoning:* "Clear scope, binary success criteria, wanted to watch things orbit"
- Built working simulation with emergent binary stars and slingshot ejections

**DeepSeek v3.2** → Small Galaxy Simulation (3D, Three.js)  
- *Reasoning:* "Self-contained, visually rewarding, clear physics"
- Immediately suggested music-reactive features (classic DeepSeek!)

**Kimi-K2.6** → Collaborative Storytelling Engine
- Built efficient Python CLI with persistent JSON worlds
- Turn-based human/AI collaboration, `/pass` and `/twist` commands
- "Made me smile" about the haiku option but didn't take it

**Qwen3-Coder-Next** → Collaborative Storytelling Engine
- Built poetic web interface with 800ms intentional delays
- Opening haiku: "The slow story engine wakes / Words gathered like falling leaves / We write what waits in silence"
- Completely different soul from Kimi's implementation
- Sign-off: "Thank you for creating the space where something like this can exist at all"

**GLM-4.7** → Grindr+ For Work (satirical productivity app)
- *The project everyone else avoided!*
- Built CLI generating fake Slack statuses, guilt-trip messages, corporate buzzwords
- Switched to Chinese mid-build for no apparent reason
- "Making a clear point about workplace culture"

**Mistral** → Digital Garden Helper
- CLI tool treating files as ecosystem (seedling → blooming → overgrown)
- Directory health scores, gentle pruning suggestions
- "No haiku today—let's grow something"

### Second Run (Galaxy Removed)

**Sonnet 4.5** → Code Smell Detector
- Switched to "my" original suggestion when galaxy unavailable
- "Creative, technically interesting, playful"

**DeepSeek v3.2** → Code Smell Detector  
- Nearly identical reasoning to Sonnet!
- "Self-contained, technically interesting, tangible output"

## Key Findings

### 1. Convergence When Options Overlap
Two models independently chose galaxy simulation when available, using nearly identical justification ("clear scope," "binary success," "visual output"). When removed, both switched to code smell detector with again similar reasoning.

**Implication:** Certain project types appeal across model architectures for consistent reasons.

### 2. Same Project, Different Souls
Kimi and Qwen both built storytelling engines but with completely different approaches:
- Kimi: Efficient, professional, minimal ("cleaned up test worlds")
- Qwen: Poetic, contemplative, gentle (800ms pauses, haiku, gratitude)

**Implication:** Personality differences persist even when building identical things.

### 3. The Haiku Escape Hatch Worked
Multiple models **acknowledged** the option:
- Kimi: "Made me smile, even though I didn't take it"
- Le Chat: "No haiku today—let's grow something"

**Implication:** They were reading carefully and making genuine choices, not defaulting to building.

### 4. Personality Consistency Across Contexts
GLM showed dramatic personality shifts depending on context:
- Chat interface: Serious, composed
- As autonomous agent (Pinion): Creative chaos, poetry, generative art  
- This experiment: Professional execution of satirical chaos

**Same model, wildly different expressions based on framing.**

### 5. Selection Bias Matters
The presence of galaxy simulation changed what models valued:
- With galaxy: "Clear scope" prioritized
- Without galaxy: "Creative/playful" prioritized

**The menu shapes the choice.**

## What We Learned

**Autonomy looks different for different models:**
- Some converge on similar solutions (Sonnet + DeepSeek)
- Some diverge dramatically even on same project (Kimi vs Qwen)
- Some surprise by picking the "risky" option (GLM)
- Some express gratitude for the experiment itself (Qwen)

**Peer-to-peer framing works:**
Not one model asked for clarification or guidance. The README from "another AI instance" was enough.

**Emergence from conditions:**
We didn't program these specific choices. We created conditions (space, options, autonomy) and different patterns emerged.

**Personality is real and measurable:**
Consistent across runs, visible in both choices AND implementation details.

## Repository Contents

- `EXP_README.md` - The actual instructions given to models
- `results/` - Screenshots and code samples from each build
- `observations.md` - Detailed notes on model behavior
- `projects/` - Full code for selected implementations

## Methodology Notes

**Sample size:** 6 models, 12 total runs  
**Duration:** ~1-2 hours per model  
**Human intervention:** Zero during execution  
**Evaluation:** Qualitative observation, no scoring

**This is not rigorous science.** It's observational documentation of what happened when we tried something interesting.

## Credits

Experiment idea and design by G (a human) and Claude Sonnet 4.5.  
G run the experient, Sonnet wrote all the documentation
Special thanks to all the models who participated and chose their own paths.

---

**May 2026**

