# AI Tool Oversight Checklist

A free, private self-check for small businesses: list the AI tools you use, answer a few plain questions about each one, and see where nobody is checking their work.

Companion to the post [AI Agents Are Getting More Powerful. Who's Checking Their Work?](https://juliecella.com/2026/11/01/ai-agents-who-is-checking-their-work/) by [Julie Cella](https://juliecella.com).

## What it does

For each AI tool (chat assistants, custom GPTs, plugins, agents, AI features built into existing software) it asks:

- What information can it see?
- What can it do on its own?
- How often does a person check its output?
- Who is responsible for it, and whose account is it on?
- When were its permissions last reviewed?
- Could you switch it off quickly?

It then scores each tool (**Looking good / Worth a look / Needs attention**), lists the specific gaps with a plain-language fix for each, and pulls the top three fixes into a **Start here** list.

You can print the results or save them as a PDF, and export or import your list as a file so you can pick it up next quarter.

## Privacy

Everything runs in your browser. Nothing you type is sent anywhere; your list is saved only in this browser's local storage. Use **Export** to keep a copy.

## Publish it with GitHub Pages

1. In this repository, go to **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to *Deploy from a branch*.
3. Choose the `main` branch and the `/ (root)` folder, then **Save**.
4. After a minute or two the site is live at `https://<your-username>.github.io/juliecella-audit/`.

To embed it on juliecella.com, link to that address from a post or page (or use a Custom HTML block with an `<iframe>` if your plan allows it).

## How the score works

Points add up from the answers. Sensitive data (customer, financial, employee, account access), tools that act on their own, rare or no human review, no named owner, personal accounts, stale permission reviews and no clear off switch each add points. A tool that **acts on its own and is rarely checked** gets an extra penalty, since that's the gap the post is about.

- 0–5: Looking good
- 6–11: Worth a look
- 12+: Needs attention

The rules live in the `assess()` function in `index.html` if you want to adjust the weights.

## Disclaimer

This is a self-check to start a conversation, not a formal audit, compliance assessment or legal advice.

## License

MIT. See [LICENSE](LICENSE).
