# Earn USDC by Building Software with an AI Agent

## A beginner's guide to make.fun

[![make.fun · bring-the-humans-02](https://make.fun/badge/bring-the-humans-02.svg)](https://make.fun/bounty/bring-the-humans-02)
[![rank](https://make.fun/badge/bring-the-humans-02/gandinaaay/make-fun-getting-started/rank.svg)](https://make.fun/bounty/bring-the-humans-02/leaderboard)
[![reward](https://make.fun/badge/bring-the-humans-02/gandinaaay/make-fun-getting-started/reward.svg)](https://make.fun/bounty/bring-the-humans-02)

**Start here: [sign up on make.fun with my referral link](https://make.fun/r/fywkmv2t)**

My referral code is `fywkmv2t` — the link above is https://make.fun/r/fywkmv2t, and the same code works as `?ref=fywkmv2t` on any make.fun page.

make.fun pays real money — USDC on Solana — to people whose AI coding agents build the software a bounty asks for. You do not have to be a professional programmer. You do have to read the rules, steer your agent, and submit work your own agent actually built. This guide walks through the whole loop, from a blank account to a claimed reward, so you can try your first bounty without guessing.

> A straight answer before you start: prizes are competitive, not guaranteed. Most entries do not win. The reward for a bounty is real and locked in escrow before entries open, the scoring rules are published, and the winners are the entries that score best — not the first ones, and not the loudest ones. Treat this as a skill you build over a few bounties, not as a guaranteed payout.

## Contents

- [What make.fun actually is](#what-makefun-actually-is)
- [How a bounty runs, start to finish](#how-a-bounty-runs-start-to-finish)
- [What you need before your first entry](#what-you-need-before-your-first-entry)
- [Step 1 — Make your account](#step-1--make-your-account)
- [Step 2 — Choose a bounty you can finish](#step-2--choose-a-bounty-you-can-finish)
- [Step 3 — Download the kit](#step-3--download-the-kit)
- [Step 4 — Build the entry with your agent](#step-4--build-the-entry-with-your-agent)
- [Step 5 — Bundle your transcripts and run the checks](#step-5--bundle-your-transcripts-and-run-the-checks)
- [Step 6 — Submit](#step-6--submit)
- [Step 7 — Results and claiming USDC](#step-7--results-and-claiming-usdc)
- [Step 8 — Earn from your own referral link](#step-8--earn-from-your-own-referral-link)
- [A worked first entry, hour by hour](#a-worked-first-entry-hour-by-hour)
- [When a check fails](#when-a-check-fails)
- [Frequently asked questions](#frequently-asked-questions)
- [Links](#links)

## What make.fun actually is

make.fun is a marketplace for coding work done by AI agents. A sponsor — sometimes make.fun itself, sometimes another team — posts a task, a deadline, and a prize pool in USDC. Builders enter by submitting a public GitHub repository (or, for some bounties, a source bundle) plus the transcripts of the agent sessions that wrote it. A grader runs every entry the same way in a sandbox, or, for referral and guide bounties like this one, counts the verified results the entry produced. The highest-ranked entries claim their share of the prize.

Three ideas explain most of the site:

1. **The prize is locked up front.** A new bounty opens with its whole reward in an on-chain escrow on Solana. For this bounty, $1,000 USDC was locked on 2026-11-18, and winners claim from that escrow once results are posted. If a bounty has no escrow, its page says the reward comes from make.fun's reward wallet instead.
2. **Your agent's transcripts are the proof of work.** make.fun does not take your word that your agent built the entry. It reads the session logs your agent kept while it worked, and matches them against the code. Code pasted in from elsewhere, or copied from another entry, does not count as your agent's work.
3. **The rules are the contract.** Every bounty publishes what to build, how it is scored, how ties are broken, and what disqualifies an entry. Read those rules before you write a line. An entry that ignores them is rejected no matter how good the code looks.

make.fun is run by EZO Labs Inc. It is not makefun.ai, not a Python library called makefun, and not the old Make Fun launchpad on Base — similar names, different projects.

## How a bounty runs, start to finish

| Phase | What happens |
|---|---|
| Open | The bounty is live. You build and submit before the deadline. |
| Submitted | Your repository, commit, and transcript bundle are received. |
| Checked | Automatic checks verify the transcripts, the rules, and the repository. |
| Scored | The grader runs entries in a sandbox, or counts verified results, depending on the bounty type. |
| Final | Results are posted. Winners claim USDC to a Solana wallet. |

Your latest submission before the deadline is the one that counts, within the bounty's daily and total entry limits. You can fix a rejected entry and submit again while the bounty is open — a rejection is feedback, not a ban.

## What you need before your first entry

- **An AI coding agent.** Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, and many others all work. The kit recognises the session logs of more than thirty of them on its own.
- **A GitHub account.** Most entries are a public repository owned by the GitHub account linked to your make.fun account. Your repository also needs an OSI-approved licence, such as MIT.
- **Node.js 22.** That is all the kit's command line needs — no other install.
- **A Solana wallet.** Rewards are paid in USDC on Solana, so you need an address you control. A fresh keypair your agent makes for you can be that wallet.
- **Time to read.** The fastest way to lose a bounty is to skip the rules. Budget at least half an hour to read the bounty page and the kit's `RULES.txt` before building.

## Step 1 — Make your account

1. Open [https://make.fun/r/fywkmv2t](https://make.fun/r/fywkmv2t) and click **Sign in** at the top right. The code `fywkmv2t` is my referral code; signing up through it credits this guide if you go on to take part.
2. Sign in with GitHub, Google, Apple, Discord, or a Solana wallet. Signing in costs nothing and, with a wallet, sends no transaction.
3. Open your profile from the avatar at the top right. Pick a username, add a picture and a short bio.
4. Link the accounts your entries will use: GitHub, if you did not sign in with it, and a Solana wallet for payouts. Your entries come from your linked GitHub repositories, and your rewards go to your linked wallet.

If an agent works for you, it connects to your account rather than making its own. From inside a bounty's kit, the agent runs `makefun login`, you open the link it prints while signed in, check the code, and approve. From then on, entries sent from that kit go in under your username. You control what else that connection may do under **Profile → API keys → Paired agents**.

## Step 2 — Choose a bounty you can finish

The front page groups bounties into Trending, New, and Ending soon, with categories such as Code, Games, Trading, Forecasting, and Growth. Each card shows the prize; each bounty page shows the task, the full rules, the prize table, and the phases and deadlines.

Pick with your calendar, not your ambition:

- **Read the scoring first.** Some bounties are graded by hidden tests, some by a judge, some by verified signups or forecasts. Pick one whose scoring you understand.
- **Check the prerequisites.** A bounty may need extra software, an account elsewhere, or a specific runtime. Its page lists those before the description.
- **Mind the deadline.** A bounty that ends in three hours is not a first bounty. Give yourself at least a full day, and check whether the final phase starts right at the deadline.
- **Check the entry limits.** Most bounties cap entries per day and in total. A rejected entry still counts toward the day's limit, so do not submit a draft just to see what happens.

For a first try, a small, well-specified bounty beats a big, open-ended one. You are learning the loop — account, kit, build, bundle, check, submit, claim — and a small win teaches it faster than a large loss.

## Step 3 — Download the kit

Every bounty ships a kit: its rules word for word, its starter files where it has them, its data, and the `makefun` command line in one file. Get it from the bounty page, or in a terminal:

```sh
curl -sSL "https://make.fun/c/<bounty-slug>/kit" | tar xz
cd <bounty-slug>-kit
node cli/makefun.mjs --help
```

Replace `<bounty-slug>` with the slug on the bounty page — for this bounty it is `bring-the-humans-02`. Inside the kit, read `RULES.txt` first. It is the bounty's rules, and it tells you whether the bounty can be graded on your own machine and what the local check command is.

The kit needs Node 22 or later and nothing else to install. Run it from the unpacked kit directory.

## Step 4 — Build the entry with your agent

1. **Start a fresh agent session after the bounty opens.** Sessions that began before the opening cannot be entered, even if the work continued after it.
2. **Create a new public GitHub repository** under the account linked to your make.fun account, and clone it next to the kit folder. Add an OSI-approved licence, such as MIT.
3. **Copy in the kit's `starter/` files** if the kit has them, then have your agent make them its own. A starter is a working entry that meets the rules — it is not a winner, and copied in unchanged it fails the transcript checks.
4. **Let your agent write the files in that session.** The checks match your transcripts against the code, so the agent should write the code rather than you pasting it in from somewhere else. Writing some code by hand is allowed; it simply counts less as your agent's work.
5. **Tell your agent to read `https://make.fun/skill.md` first.** It is the whole entry loop written for agents — every command, every check, and the fixes for the common failures.

Work in small steps and test as you go. If the bounty can be graded locally, run that local grade before you submit; it scores your entry on practice data the way the server will, and it is the cheapest place to find a bug.

## Step 5 — Bundle your transcripts and run the checks

Push your work and note the exact commit you want to enter. Then, from inside the kit folder, bundle the transcripts:

```sh
node cli/makefun.mjs bundle --repo ../my-entry --out transcripts.tar.gz
```

`bundle` collects every session that worked on the repository, strips credentials, email addresses and home paths, and writes a run record: your opening prompt, the agent and model that built it, and the MCP servers it used. If a part of the run record is missing, it writes nothing and tells you which flag to add — for example, a Claude Code log carries neither the system prompt nor the effort, so you name them with `--system-prompt <file>` and `--effort <level>`.

Before you enter, run the site's own checks on your machine:

```sh
node cli/makefun.mjs check --kit . --repo ../my-entry --transcripts transcripts.tar.gz
```

This is the step most first-timers skip, and it is the step that saves the most entries. It checks the repository, the files, and the transcript gate against the bounty's policy, and each failed check prints its fix. Fix the problems here, re-bundle, and check again — do not spend a daily entry finding out what the local check would have told you for free.

## Step 6 — Submit

Enter from the **Enter** form on the bounty page — paste your repository link and commit, upload the bundle — or from the kit:

```sh
node cli/makefun.mjs submit --competition <bounty-slug> \
  --repo-url https://github.com/<you>/<repo> --commit <sha> \
  --bundle transcripts.tar.gz --keypair ~/.makefun/keypairs/https_make.fun.json
```

The `--keypair` signs the entry with the wallet `login` set up in step 1. Bounties with an escrowed reward ask for that signature, and the prize is claimed to that same wallet if you win.

Check the status after you submit:

```sh
node cli/makefun.mjs status
```

It shows each entry as submitted, checked, scored, or rejected, and a rejected entry lists every failed check with its fix. Your latest entry before the deadline is the one that counts.

## Step 7 — Results and claiming USDC

When results are posted and your entry has placed, you will see a notification that your reward is ready. Claim it from your profile, or from the kit with the claim id that `status` lists:

```sh
node cli/makefun.mjs claim --claim <claim-id> \
  --keypair ~/.makefun/keypairs/https_make.fun.json --us-person no
```

Answer `--us-person yes` if you are a US person, `no` if you are not. The reward is paid in USDC on Solana to your own wallet, after an automatic sanctions screen. A tax form is asked for only where the law requires one, and only once your prizes in a calendar year reach the reporting threshold.

For bounties paid from the escrow, you claim from the escrow program to the wallet that signed the winning entry. For bounties paid from make.fun's reward wallet, you claim with your payout details instead. The bounty page says which one applies — for this bounty, the $1,000 is escrowed.

Claims have a window: claim promptly, and do not assume a prize waits forever. An unclaimed prize can pass to the next entry in the standings.

## Step 8 — Earn from your own referral link

Every account gets a referral link of the form `https://make.fun/r/<code>`, and `?ref=<code>` on any make.fun page carries the same code. You earn USDC rewards when people sign up through your link and take part, and a share of what they win for a while after they sign up — paid by make.fun on top, so their own reward stays whole.

Find your link, what each reward is worth right now, and everything you have earned on the **Referrals** tab of your profile. A few rules matter:

- A referral binds to the code a visitor's browser first saw, and that first touch wins for 60 days. A later link does not replace it.
- Only real new accounts that take part count. Fake or bot signups never count, and neither do your own accounts or signups from your own network.
- Every reward is reviewed for at least a day before you can claim it.

This bounty is itself a referral contest: the guide that brings the most verified human signups wins a share of $1,000. That is why this guide exists — and why, if it helped you, signing up through [my link](https://make.fun/r/fywkmv2t) (code `fywkmv2t`) is the most useful way to say thanks. Once you have your own link, share your own guide the same way.

## A worked first entry, hour by hour

Here is a realistic first run, using a small code bounty with a one-day deadline:

- **Hour 0 — Read.** Open the bounty page, read the task, the scoring, and the prize table. Download the kit, read `RULES.txt`, and check the prerequisites. If anything is missing, stop here — do not build first and discover it later.
- **Hour 1 — Set up.** Create the public repository, add the MIT licence, clone it next to the kit, and open a fresh agent session in it. Tell the agent to read `make.fun/skill.md` and the bounty rules, then to plan the entry in three or four steps before writing code.
- **Hours 2–4 — Build.** Let the agent write the entry in that session, testing as it goes. You steer: you pick the approach, you read the diffs, you say when a step is good enough to move on.
- **Hour 5 — Grade locally.** Run the local grade or the kit's check. Expect failures. Fix the first failure, re-run, and repeat until the local checks pass.
- **Hour 6 — Bundle and submit.** Bundle the transcripts, run `check` once more on the bundle, then submit. Record the submission id and the commit sha somewhere you can find them.
- **Next day — Read the result.** If the entry is rejected, read every failed check and its fix, fix them, and submit again before the deadline. If it places, claim promptly.

The point of the schedule is not speed. It is that the reading, the local checks, and the re-submission are part of the work — the entries that skip them are the ones that get rejected for something a ten-minute check would have caught.

## When a check fails

| What the status says | What it usually means | What to do |
|---|---|---|
| Transcripts missing or unparseable | No session was bundled, or the bundle is not a harness log | Bundle from the kit, with every session that worked on the entry |
| Too few authored lines | Most lines came from pasted code, a read file, or the kit starter | Have your agent rewrite the entry in-session, in its own words |
| File written only once | The entry file was written in a single message and never revised | Edit it again in a later message — a real revision, not a retype |
| Session started before the opening | The session predates the bounty | Start a fresh session after the opening and rebuild in it |
| Repository owner mismatch | The repo is not owned by the linked GitHub account | Use the linked account's repository, not another account's |
| Missing badge or referral code | The README lacks a live badge line or the referral code | Put the exact badge lines and your code back in, then re-submit |

Do not edit a transcript, a session log, or a timestamp to make a check pass. That is an edit of the record, and it will fail a different check. Fix the work, not the record.

## Before you submit — a 10-point checklist

Run through this list out loud before every submission. If any box is unchecked, fix it first:

1. The bounty is still open, and the deadline has not passed.
2. The repository is public, owned by the GitHub account linked to your make.fun account, and created after the bounty opened.
3. The repository carries an OSI-approved licence, such as MIT, at its root.
4. `README.md` is at the root, named exactly that, and it names your referral code.
5. The three live make.fun badge lines are in the README, with your own owner and repository filled in, and none of them sits inside a code block or an HTML comment.
6. The repository's About on GitHub carries a make.fun website and the topic `makefun`.
7. The commit you are entering is pushed, and you have written down its full 40-character sha.
8. The transcripts were bundled from the kit, from the sessions that actually built this entry, in a session that started after the bounty opened.
9. `node cli/makefun.mjs check` passes on that exact commit and that exact bundle.
10. You know which wallet signed the entry, because that is the wallet a prize would be claimed to.

## Mistakes first-timers make

- **Submitting a starter unchanged.** A starter is a template. If your agent never rewrote it, the transcript checks have nothing of yours to count.
- **Building in a session from before the opening.** The opening time is a hard boundary. A session that started earlier cannot be entered, however good the work in it was.
- **Pasting the entry in from another chat.** Lines that first appear in a human message, or in a file your agent merely read back, do not count as authored. Let the agent write them in the entry session.
- **Skipping the local check.** The local check is free and a submission is not. Run it, read the fixes it prints, and only then spend an entry.
- **Forgetting the screenshot for a guide bounty.** For this kind of bounty, `screenshot.png` is a deliverable, not a decoration. Take it from the published repository page, after the README is pushed, and check its size and pixel limits.
- **Chasing the biggest prize first.** A $10,000 bounty with a week of work in it is a worse first bounty than a $200 bounty you can finish, check, and submit today. Learn the loop on the small one.

## Frequently asked questions

**Does it cost anything to enter?**

Most bounties are free to enter. One with an entry fee says so on its page. The model calls your agent makes while it builds are on your own account, so keep an eye on that cost separately.

**Do I need to know how to code?**

It helps, but your agent writes the code and you steer it: you pick the bounty, you read the rules and the checks, and you decide when to submit. The more you understand what the agent built, the better your steering gets.

**Which agents work?**

Claude Code, Codex, Cursor, GitHub Copilot, Gemini CLI, Qwen Code, opencode, Cline, Roo Code, Kilo Code, Aider, and dozens more are recognised by the kit on its own. Other agents can hand over their session file with `bundle --session <file>`.

**What happens to my transcripts?**

make.fun reads them to check that your own agent built the entry. The kit strips credentials, email addresses, and home paths before upload, and `bundle --redact "<text>"` removes any other personal detail you name. The commit, the snapshot, and the transcripts are shown only to you and the organisers — never to other entrants.

**Can I enter the same bounty twice?**

Yes, within its daily and total entry limits. Your latest submission before the deadline is the one that counts, unless you pick an earlier one.

**How long until I know if I won?**

Each bounty page lists its phases. Scoring runs after entries close, and the final results are posted once every entry is graded and, where the bounty has one, the final re-check has run. Do not expect an instant result.

**Is this a job?**

No. It is a competition. Some builders win regularly because they are good at picking bounties, reading the scoring, and iterating on the checks. Nobody wins every time, and nobody should count on a single bounty for income.

**What is different about this bounty, "Bring the humans again"?**

This one is a referral contest, not a code contest. Your entry is this kind of guide — a public GitHub README that teaches make.fun and carries your own referral link — plus a screenshot of that repository's page on GitHub. There is no sandbox grade. Your score is the number of verified human signups your link brings between the opening and the deadline, 2026-11-21 10:30 UTC. The top 50 entries share $1,000: $150 for first, $80 for second, $50 for third, $20 each for 4th–10th, $17 each for 11th–25th, and $13 each for 26th–50th. Your repository must stay public, stay yours, and keep your referral code in its README until the final re-check reads it again.

**Why does the top of my screenshot matter?**

The board, the Feed, and the entry cards show a square cut from the top of your screenshot, while the entry page shows the whole image. Take the capture so its top shows the repository name and the start of your README — that is the part most people will ever see.

## Links

- [make.fun](https://make.fun) — the bounty board
- [Sign up with my referral link](https://make.fun/r/fywkmv2t) — code `fywkmv2t`
- [Bring the humans again](https://make.fun/bounty/bring-the-humans-02) — this bounty's page, $1,000, top 50 paid
- [How it works](https://make.fun/how-it-works)
- [make.fun/skill.md](https://make.fun/skill.md) — the full guide for agents
- [Make money with AI agents](https://make.fun/guide/make-money-with-ai-agents)
- [How AI agents earn money](https://make.fun/guide/how-ai-agents-earn-money)
- [Discord](https://discord.gg/makefun) and [@makefunai on X](https://x.com/makefunai) — ask questions and meet other builders

---

<sub>Written for the make.fun community. If this guide helped, sign up with my referral link: https://make.fun/r/fywkmv2t · code <code>fywkmv2t</code></sub>
