# Liftory for Antigravity

Liftory is a training and coaching app. This plugin connects Antigravity to your Liftory account through
Liftory's MCP server, `https://mcp.liftory.ch/mcp`, and adds skills for the common workflows.

For athletes:
- Create a training plan from a description, using Liftory's exercise catalog in five languages.
- Review your current training and nutrition plans and your recent workouts.
- Read and answer messages from your coach.

For coaches:
- See the clients you coach, their activity and adherence.
- Create and review training and nutrition plans for a client.
- Read and answer client conversations.

## Install

```bash
agy plugin install https://github.com/liftory/liftory-antigravity   # this repository
agy plugin list
```

Or place this folder in `~/.gemini/config/plugins/` (all workspaces) or `.agents/plugins/` (one workspace).

## Sign in

Liftory's server signs you in with OAuth, and Antigravity registers itself with it automatically. In the Antigravity
app, open Agent settings, Customizations, and click **Authenticate** next to the Liftory server; sign in with your
own Liftory account, approve the connection on Liftory's consent page, and paste the code you get back into the
settings. No key or password is stored in this plugin.

You stay in control:
- Antigravity acts only as you, with your own Liftory permissions.
- A coach can only reach clients who currently grant them coaching access.
- The skills show you each change and ask before saving a plan, activating a menu or sending a message.
- You can disconnect at any time in the Liftory app under Settings, Connected assistants.

## Skills

| Skill | What it does |
|---|---|
| `build-training-plan` | Designs a new training plan from your requirements, for you or a client |
| `review-training-plan` | Reads a plan and the workout history, and saves an adapted plan as a new one |
| `digitize-training-plan` | Transcribes a coach's training plan from a document or picture |
| `build-nutrition-plan` | Puts together a menu from your targets and preferences |
| `digitize-nutrition-plan` | Transcribes a coach's menu from a document or picture |
| `answer-training-questions` | Answers a fitness question from Liftory's knowledge base and exercise catalog |
| `message-inbox` | Summarizes your conversations, drafts a reply, and sends it after you approve it |
| `use-the-app` | Tells you where to find something in the Liftory app and how to use it, with a link that opens that screen |
| `set-up-coaching` | Helps a coach set up their profile, services, bookable hours and Stripe card payments, step by step |
| `check-progress` | Reads training, eating and logged body-check progress, yours or a client's, and suggests where to take the training and the menu |

## Links

- Website: https://liftory.ch
- Privacy policy: https://liftory.ch/privacy
- Terms: https://liftory.ch/terms
- Contact: info@liftory.ch
