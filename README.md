# 36leads

Finds new customers: clarifies your ideal customer, finds target companies and contacts, and adds them to a 36leads campaign, right in your chat with Claude or Codex.

Requires a [36leads](https://36leads.io) account with contact search enabled.

## Installation

**Claude Code**

```bash
claude plugin marketplace add 36leads/36leads-plugin
claude plugin install 36leads@36leads
```

Sign in with your 36leads account on first use.

**Codex**

```bash
codex plugin marketplace add 36leads/36leads-plugin
codex plugin add 36leads@36leads
codex mcp add 36leads --url https://app.36leads.io/api/mcp/mcp
codex mcp login 36leads
```

Then start a new session.

## Usage

Say that you are looking for more customers, or name companies or people directly. The assistant uses what your project folder already says about your offer and works through your 36leads account.

## Data

The plugin reads information about your offer and your customers in the current project folder. It sends your target profile, companies and people to your 36leads account via `https://app.36leads.io/api/mcp/mcp`. Sign-in uses OAuth; the plugin contains no credentials.
