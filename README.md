# Viola Decision Coach v1.0

A reusable AI skill trained on Viola's approach to breaking down vague leadership requests into concrete next steps.

## Files

- `SKILL.md` — core behavior, principles, playbooks and response instructions.
- `references/decision-principles.md` — expanded reasoning patterns and boundaries.
- `references/training-cases.md` — grounded examples from the training conversations.
- `templates/request-breakdown.md` — a practical first-pass action plan.
- `templates/decision-brief.md` — format for bringing options and recommendations to a manager.

## Install in Claude (native Skill)

1. Open Claude and enable **Create and edit files** if requested (Settings → Capabilities).
2. Go to **Customize → Skills** and select **+ → Create skill → Upload a skill**.
3. Upload the ZIP package (`Viola_Skill_v1.zip`) without unzipping it.
4. Enable the skill, then ask: "My boss asked me to improve xPods subscriptions. Help me figure out where to start."

The archive includes the folder `viola-decision-coach/`, matching the `name` in the skill metadata. Team and Enterprise admins may share or provision the skill centrally.

## Use in ChatGPT (Project)

1. In ChatGPT, create a Project called **Viola Decision Coach**.
2. Add the standalone `Viola_Skill_v1.md` file to the Project's sources, or upload `SKILL.md` plus the two reference files from this package.
3. In **Project settings → Instructions**, paste:

> Follow the uploaded Viola Skill as your primary coaching method for interpreting vague leadership requests. Start by clarifying the real business/customer objective and suggesting practical next steps, workstreams, owners, and possible escalations. Be grounded, commercially aware, respectful of decision authority, and candid about unknowns. Do not impersonate Viola or invent xBloom facts.

4. Keep all related questions within the Project. You may share the Project with the team, but remember that project members can see shared project conversations and files.

## Use in Gemini (Gem)

Create a new **Gem** in Gemini, use the short Project instruction above as its instructions, and upload the standalone `Viola_Skill_v1.md` under Knowledge. Save and test. Gems can be shared where enabled.

## Scope and review

The skill is an approximation of Viola's decision-making, not a replacement for company policy, fact verification or leadership approvals. Examples include internal commercial practices and historical benchmarks; distribute only to appropriately authorized colleagues. Update after testing against real requests and reviewing corrections.
