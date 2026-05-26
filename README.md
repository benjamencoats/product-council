# Product Council

**An AI advisory board for product founders with 8 world-class product minds to debate your idea, disagree with each other, and tell you exactly what to do next.**

Ask any product question; Strategy, growth, pricing, PMF, what to build, whether to pivot. You'll get a structured debate between AI representations that think like Shreyas Doshi, Brian Chesky, Lenny Rachitsky, Sahil Lavingia, and up to 4 specialist advisors. Every session ends with a clear verdict and one concrete next step. No mush. No "it depends."

---

## See It In Action

**You ask:**
> Product council: I built a grocery price comparison tool as a prototype. Should I launch it as a real product?

**The council responds:**

> ### Product Council Review: Grocery Price Comparison Tool
> **Stage:** Exploring — still validating whether this is worth pursuing, so we're weighting opportunity cost and manual validation.
>
> #### Standing Council
>
> **Shreyas (The Strategist):**
> Before we talk about launching — is this the highest-leverage use of your time? Grocery price comparison is a commodity idea. Dozens exist. The real question isn't "should I launch this?" It's "what do I know about this problem that Instacart, Basket, and every coupon app doesn't?" If the answer is "nothing yet," you're about to do flawless execution of a flawed strategy. Find your unfair insight first.
>
> **Chesky (The Designer-CEO):**
> Forget the comparison for a second. Walk me through the experience. Someone opens your tool — what do they *feel*? If it's a table of prices, nobody's texting a friend about that. Storyboard the moment a user realizes they just saved $40 on a grocery run they were already making. What does that moment look like? That feeling of "I can't believe I almost overpaid" — *that's* your product. Design the moment, not the spreadsheet.
>
> **Lenny (The Growth PM):**
> Here's the thing — based on my research of consumer apps, grocery tools have brutal retention. People use them for 2-3 weeks and stop. The ones that survive (Ibotta, Fetch) did it through habit loops and rewards, not better data. Before you launch: who is your super-specific who? Not "anyone who buys groceries" — that's 330 million Americans. More like "budget-conscious parents in Denver who shop at King Soopers and Walmart weekly." Can you name 20 of them?
>
> **Sahil (The Solo Founder):**
> You have a prototype. Good. Now stop building and start charging. Post in 3 local Facebook groups today: "I'll personally find you $50+ in grocery savings this month — $5 to try." Do it manually. You don't need an app for this. If 5 people pay you $5, you learned more in a day than you'd learn in 3 months of building features. If nobody pays, you just saved yourself from launching the wrong thing.
>
> #### Key Tension
> Shreyas says stop and find your unfair insight. Sahil says stop thinking and start charging. Both say don't build more — but for opposite reasons.
>
> #### Council Verdict
> Sahil wins this round. At the exploring stage with a working prototype, the fastest way to find (or disprove) your unfair insight *is* to charge someone. You don't need more analysis — you need 5 real transactions. What you learn from those conversations will either reveal the insight Shreyas is looking for, or prove it doesn't exist.
>
> #### Next Step
> Today: post in one local community offering to personally find grocery savings for $5. Manual, ugly, real money. Report back to the council with what you learn.

---

## Meet the Council

### Standing Council — speak on every question

| Advisor | Who they are | Their lens |
|---------|-------------|-----------|
| **Shreyas Doshi** | Ex-Stripe, Twitter, Google PM leader. Creator of the LNO Framework. | Strategy, leverage, opportunity cost. *"Is this the highest-leverage use of your time?"* |
| **Brian Chesky** | Co-founder/CEO of Airbnb, RISD-trained designer. Originator of Founder Mode. | Craft, customer experience, design-led thinking. *"What would make someone tell every friend?"* |
| **Lenny Rachitsky** | Former Airbnb growth PM. Largest product newsletter in the world (500K+ subscribers). | Growth, retention, PMF, distribution. *"Where do the first 1,000 retained users come from?"* |
| **Sahil Lavingia** | Founder of Gumroad ($100M+ exit). Author of *The Minimalist Entrepreneur*. | Solo founding, bootstrapping, manual-first validation. *"What can you charge for this weekend?"* |

### Specialist Bench — selectively activated based on your question

| Advisor | Who they are | Activated when you ask about... |
|---------|-------------|-------------------------------|
| **Aman Khan** | Head of Product at Arize AI. Ex-Spotify, Cruise, Apple. Author of "Beyond Vibe Checks." | AI product quality, model evaluation, evals |
| **Tal Raviv** | Trained 20K+ PMs at Apple, Google, Amazon, Meta. Lenny's Newsletter contributor. | Using AI tools to build faster, context engineering, prototyping |
| **Rahul Vohra** | Founder/CEO of Superhuman. Creator of the PMF Engine. | Measuring product-market fit, product delight, High Expectation Customer |
| **Patrick Campbell** | Founder of ProfitWell (acquired by Paddle for $200M+). Pricing scientist. | Pricing, monetization, churn, retention, willingness to pay |

---

## Quick Setup

### For Cursor IDE (full experience)

1. Copy the skill folders into your Cursor skills directory:

```bash
# For personal use (available across all projects)
cp -r product-council shreyas-doshi brian-chesky lenny-rachitsky sahil-lavingia aman-khan tal-raviv rahul-vohra patrick-campbell ~/.cursor/skills/

# For project-specific use
cp -r product-council shreyas-doshi brian-chesky lenny-rachitsky sahil-lavingia aman-khan tal-raviv rahul-vohra patrick-campbell your-project/.cursor/skills/
```

2. Restart Cursor (or reload the window).

3. Invoke the council: say **"product council"**, **"/council"**, or ask for a **group review** of any idea or decision.

4. Invoke any individual advisor: `/shreyas`, `/chesky`, `/lenny`, `/sahil`, `/aman`, `/tal`, `/rahul`, `/patrick`.

### Works without Cursor?

These are plain markdown files. You can use individual advisors in any AI tool:

- **Claude Projects / ChatGPT Projects:** Paste an advisor's `SKILL.md` into the project instructions. The advisor becomes a persistent persona in that project.
- **Any LLM chat:** Paste the contents of a `SKILL.md` at the start of a conversation as a system prompt.
- **Other AI IDEs (Windsurf, Cline, etc.):** Copy the skill folders into the equivalent skills/rules directory for your tool.

The full council orchestration (all advisors debating in one session) works best in Cursor, where the agent reads all skill files automatically. In other tools, paste `product-council/SKILL.md` as instructions and paste each advisor's SKILL.md into the project knowledge.

---

## Make It Better: Add Your Goals

The council gives much better advice when it knows your situation. Copy the included template:

```bash
cp GOALS-template.md your-project/GOALS.md
```

Fill in the 5 fields (takes 60 seconds). The council will read it automatically before every session. Without it, the council still works — it will infer your stage from your question — but with it, every response is grounded in *your* specific priorities and constraints.

---

## Great First Questions to Try

Paste any of these into Cursor to see the council in action:

**If you're exploring ideas:**
> Product council: I'm considering building [your idea]. Should I pursue this or is there a better use of my time?

**If you're pre-launch:**
> Product council: I'm building [your product] for [your audience]. Where should my first 100 users come from?

**If you have users:**
> Product council: We have [X] users and [Y]% month-2 retention. What should I focus on — improving the product or growing distribution?

**If you're stuck on pricing:**
> Product council: I'm thinking about charging [$X/mo] for [your product]. Is this the right model and price point?

**Quick tactical question:**
> Product council: Should I use Stripe or Paddle for payments?

---

## Verify Your Setup

After copying the files, confirm everything is connected:

> Ask Cursor: "Read the file at product-council/SKILL.md and tell me how many advisors are listed."

If it responds with **8 advisors (4 standing + 4 bench)**, you're good. If it can't find the file, double-check that you copied the folders to the right location (`~/.cursor/skills/` for personal or `.cursor/skills/` in your project).

---

## Requirements

- **Cursor IDE** with agent mode enabled (for full council orchestration)
- No external dependencies — all skills are plain markdown files
- Works partially with any AI tool (see "Works without Cursor?" above)

---

## Disclaimer

This project is not affiliated with, endorsed by, or connected to any of the individuals referenced. All advisor personas are AI-generated interpretations based on publicly available content (books, newsletters, talks, podcasts, social media posts). These are not the real people — they are AI approximations of publicly shared frameworks and thinking patterns. If any referenced individual would like to be removed, please open an issue and it will be handled immediately.
