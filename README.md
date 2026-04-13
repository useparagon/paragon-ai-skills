<p align="center">
  <a href="https://www.useparagon.com/" target="blank"><img src="https://raw.githubusercontent.com/useparagon/aws-on-prem/master/assets/paragon-logo-dark.png" width="150" alt="Paragon Logo" /></a>
</p>

<p align="center">
  <b>
    The embedded integration platform for developers.
  </b>
</p>

---

# Paragon Skills
Agents can **set up your integrations** in just minutes with Paragon Skills. The Paragon Skill provides your agent context with everything it needs to:

1. Set up the Paragon SDK

2. Add the Connect Portal to authenticate your users 

3. Get started with [ActionKit](https://useparagon.com/product/actionkit), [Managed Sync](https://useparagon.com/product/managed-sync), and [Workflows](https://docs.useparagon.com/workflows/overview) to build any integration use case.

If you're setting up Paragon for the first time, use this Skill to get up and running with your integrations.

![Paragon Skill](/assets/opencode-skill.png)

## Getting Started

### Recommended: Installing via the Skills CLI
The `npx skills` CLI by Vercel automatically adds the Paragon Skill for the most popular agentic IDEs.

```bash
npx skills add useparagon/paragon-skills
```

Update the Paragon Skill with the following command:

```bash
npx skills update
```


### Alternative: Manual Installation
1. Navigate to the `skills/` directory for your agentic IDE of choice, e.g.

```bash
~/.cursor/skills/
~/.claude/skills/
~/.agents/skills/
~/.config/opencode/skills/
```

2. Clone the [Paragon Skills Repo](https://github.com/useparagon/paragon-skills) in the `skills/` directory:

```bash
git clone https://github.com/useparagon/paragon-skills.git
```

## Using the Skill
Your agent should naturally detect when the Paragon Skill is needed.

In some cases, it may be useful to reference the skill directly by name (i.e. "Using the Paragon Setup Skill..." or "/paragon-setup-skill").

### Starter Prompts

```markdown
/paragon-setup-skill Look at my app and set up the Paragon SDK, including all dependencies and required setup steps.

I will provide the following environment variables for your reference:
- `PARAGON_PROJECT_ID`: The Paragon Project UUID.
- `PARAGON_SIGNING_KEY`: The Signing Key as a PKCS8-encoded private key.
```

```markdown
/paragon-setup-skill Build an integration catalog for the integrations defined in my Paragon project.
```

```markdown
/paragon-setup-skill Set up auth for using the Paragon SDK.
```

