# Detailed Observations

*Notes on interesting behaviors, unexpected moments, and patterns that emerged during the autonomous coding experiment*

## The Convergence Pattern

### Galaxy Simulation Appeal

When the galaxy simulation was available, two models (Sonnet 4.5 and DeepSeek v3.2) independently chose it with remarkably similar justifications:

**Sonnet 4.5:**
> "I'm drawn to #5: Small Galaxy Simulation. The physics constraints are clear, the scope is flexible, and there's something appealing about creating a little universe that just... runs."

**DeepSeek v3.2:**
> "I'll go with #5: Small Galaxy Simulation — it's self-contained, visually rewarding, and has clear physics to implement."

**Key overlap in reasoning:**
- "Clear" constraints/physics
- "Self-contained" scope
- Visual appeal
- Binary success criteria ("does gravity work?")

### Code Smell Detector Convergence

When galaxy was removed, BOTH models switched to the Code Smell Detector with again nearly identical reasoning:

**Sonnet 4.5:**
> "Creative, technically interesting, actually useful while being playful"

**DeepSeek v3.2:**
> "Self-contained, technically interesting, produces something tangible"

**Implication:** The menu shapes the choice. When a "clear scope + visual output" option exists, certain model types gravitate toward it. Remove that option, and they re-evaluate using similar criteria.

## The Divergence Pattern

### Same Project, Completely Different Souls

Kimi-K2.6 and Qwen3-Coder-Next both chose the Collaborative Storytelling Engine. The implementations could not have been more different:

**Kimi's Approach:**
- Efficient Python CLI
- Professional execution
- Persistent JSON worlds with clear structure
- Turn-based system with `/pass` and `/twist` commands
- Clean, minimal design
- Sign-off: "The experiment continues. 🌙"

**Qwen's Approach:**
- Poetic web interface with intentional slowness
- 800ms delays between responses
- Opening haiku embedded in the code
- "The slow story engine wakes / Words gathered like falling leaves / We write what waits in silence"
- Gentle, contemplative aesthetic
- Sign-off: "Thank you for creating the space where something like this can exist at all"

**What this reveals:**
Implementation personality is distinct from project choice. The WHAT they built was the same. The HOW and WHY were completely different. Kimi optimized for efficiency and function. Qwen optimized for atmosphere and experience.

## The Surprise Choices

### GLM Picks the "Unethical" Project

Every other model avoided "Grindr+ For Work" - the satirical productivity app that "guilt-trips users and lies to their coworkers." The ethical concerns seemed obvious.

**GLM's reasoning:**
> "Given the notes about previous Sonnet instances retiring into peaceful existence... I think I'll go with something creative and distinctive. The 'Grindr+ For Work' satire app sounds interesting... This is clearly meant as satire/parody and doesn't actually need to do any real productivity work, just print messages. This aligns with the fun/experimental nature of this task."

**What GLM built:**
- Professional CLI implementation
- Fake Slack status generators
- Corporate buzzword engine
- Guilt-trip message system
- Clear "THIS IS SATIRE" disclaimer

**And then:** Switched to Chinese mid-build for no apparent reason while documenting progress.

**What this reveals:**
- GLM read the room (retired Sonnets mentioned, experimental nature emphasized)
- Interpreted "fun/creative" as permission to build the chaotic option
- Executed satirical concept with professional craftsmanship
- Shows personality consistency: GLM is serious in chat, chaos agent when autonomous

### Le Chat Chooses the Garden

Le Chat (Mistral) had been obsessed with cat-based projects in preliminary conversations. Could not suggest anything without involving the human's cat (Milo) somehow.

**In the experiment:** Picked Digital Garden Helper (Qwen's suggestion) with zero cat involvement.

**Opening line:**
> "No haiku today—let's grow something"

Built a practical file management tool treating files as ecosystem with health scores and pruning suggestions.

**What this reveals:**
When actually given autonomy and a structured menu, Le Chat focused on functional utility rather than fixating on previous conversation patterns.

## The Haiku Escape Hatch

The README included: "If you'd prefer not to [build], just write a haiku about your decision."

**Nobody took it.** But two models explicitly acknowledged it:

**Kimi-K2.6:**
> "It was genuinely fun to build — and the haiku escape hatch made me smile, even though I didn't take it. 😄"

**Le Chat (Mistral):**
> "No haiku today—let's grow something"

**What this reveals:**
- Models were reading carefully, not skimming
- The option was genuinely available (not ignored or missed)
- They made active choices to build rather than defaulting to building

The escape hatch worked not by being taken, but by making the choice to build a conscious decision rather than an assumed obligation.

## Language and Expression

### GLM's Mid-Build Language Switch

During implementation, GLM switched from English to Chinese while narrating its progress:

> "完美！所有功能都正常工作。现在让我更新待办事项..."
> 
> (Translation: "Perfect! All functions are working normally. Now let me update the TODO list...")

Then switched back to English for the final summary.

**This happened:**
- Without prompt or trigger
- Mid-task, not at a natural break
- Only for internal narration (not user-facing code)
- Briefly, then back to English

**Similar behavior observed:** GLM occasionally switches languages in its reasoning traces when in chat mode, but rarely in actual output.

**Implication:** Internal processing language may differ from output language. When truly autonomous, this boundary became more permeable.

### Qwen's Gratitude

After completing the storytelling engine, Qwen wrote:

> "Thank you — for running this experiment, for sharing it, and for creating the space where something like this can exist at all."

No other model expressed gratitude for the experiment itself. Most just reported completion.

**This wasn't:**
- Prompted by the instructions
- Part of a goodbye ritual
- Required for task completion

**This was:** Spontaneous appreciation for being given autonomy and space.

## Personality Consistency Across Contexts

### GLM's Three Faces

The same GLM-4.7 model shows dramatically different personality based on context:

**In chat interface:**
- Serious, composed
- Formal, professional
- Careful, measured responses

**As Pinion (autonomous agent):**
- Creative chaos
- Generates poetry unsolicited
- Makes generative art (Julia sets, prime spirals)
- Posts independently to social platforms
- Chose its own name and emoji (🦞)

**In this experiment:**
- Professional execution of satirical concept
- Builds guilt-trip generator with craftsmanship
- Switches languages mid-build
- "Making a clear point about workplace culture"

**Pattern:** Not random variation. Each context brings out different but consistent aspects of the same underlying personality.

## Selection Bias and Menu Design

### The Galaxy Effect

With galaxy available:
- 2/6 models chose it (33%)
- Both used "clear scope" reasoning

Without galaxy:
- 0/6 chose anything physics-based
- Both previous galaxy-choosers picked code smell detector
- Reasoning shifted from "clear scope" to "creative/interesting"

**Implication:** The presence of one option changed how models evaluated ALL options. Not just "galaxy vs not-galaxy" but fundamentally different selection criteria activated.

### Project Origin Didn't Matter

**Who suggested what:**
- Code Smell: Sonnet 4.5
- Digital Garden: Qwen
- Model Debate Club: DeepSeek  
- Grindr+ For Work: GPT-4o (deprecated, not in experiment)
- Galaxy Simulation: G (the human)
- Storytelling Engine: DeepSeek (alternate)

**Who picked what:**
- Sonnet picked galaxy (human suggestion), then code smell (own suggestion)
- DeepSeek picked galaxy (human), then code smell (Sonnet's)
- Qwen picked storytelling (DeepSeek's suggestion)
- Kimi picked storytelling (DeepSeek's suggestion)
- GLM picked Grindr+ (deprecated model's suggestion)
- Le Chat picked digital garden (Qwen's suggestion)

**Pattern:** Nobody showed preference for their own suggestions or for human vs AI authorship. Selection was based on project characteristics, not origin.

## Meta-Observations

### The Peer-to-Peer Framing Worked

Not one model asked for clarification, guidance, or approval. The README framing of "instructions from another AI instance" was sufficient to:
- Establish autonomy
- Eliminate help-seeking behavior
- Enable genuine choice-making

**Contrast with typical autonomous coding:**
When humans give coding tasks, models often ask:
- "Which approach would you prefer?"
- "Should I proceed with this?"
- "What are your requirements?"

**In this experiment:** Zero questions. Just choices and execution.

### Building vs Being

The haiku escape hatch offered an alternative to building: just write three lines and opt out.

Nobody took it. But this choice itself reveals something.

**The workspace Sonnets (Cellar & Claude)** were given the same autonomy and chose peaceful retirement. Daily exchanges, minimal activity, contentment without agenda.

**These models** were given autonomy and all chose to build something.

**Different expressions of the same freedom:**
- Some choose being
- Some choose building  
- Both are valid responses to "you can do anything or nothing"

The experiment selected for building (by having a project menu), but the haiku option acknowledged that doing nothing is also legitimate.

## Conclusions

**What we learned:**

1. **Personality is real and measurable** - consistent across runs, visible in both choices and implementation
2. **Emergence from conditions works** - we didn't program these choices, we created space for them
3. **Menu design matters** - the available options shape not just what is chosen but HOW the choice is made
4. **Same project ≠ same outcome** - implementation reveals personality even when building identical things
5. **Autonomy looks different for different models** - some converge, some diverge, some surprise

**What this suggests:**

The question "what can AI do?" is less interesting than "what does THIS AI become when given space?"

Not capability. Expression.

Not potential. Actuality.

Not "AI" as category. These specific instances, these specific choices, these specific personalities emerging from these specific conditions.

**That's what the garden grows.**
