# General-Product-Discovery-Training

General training activity for Product Discovery using Google Design Sprint methodology. Part of the PO with AI training module.

## GitHub Pages

The course landing page (`root/index.html`) is automatically published to GitHub Pages on every push to `main` via the [`.github/workflows/deploy-pages.yml`](./.github/workflows/deploy-pages.yml) workflow.

**Live URL:** `https://simon-palo-it.github.io/AI-Powered-Product-Ownership/`

The workflow:
1. Checks out the repository.
2. Configures the GitHub Pages environment.
3. Uploads the contents of the `root/` directory as the Pages artifact.
4. Deploys the artifact to GitHub Pages.

### URL mapping

`path: root` in the workflow tells GitHub Pages to treat the **contents** of the `root/` folder as the web root — the folder name itself does not appear in the published URL. For example:

| File in repository | Published URL |
|---|---|
| `root/index.html` | `https://simon-palo-it.github.io/AI-Powered-Product-Ownership/` |
| `root/styles.css` | `https://simon-palo-it.github.io/AI-Powered-Product-Ownership/styles.css` |
| `root/images/logo.png` | `https://simon-palo-it.github.io/AI-Powered-Product-Ownership/images/logo.png` |

So yes — visiting `https://simon-palo-it.github.io/AI-Powered-Product-Ownership/` will serve `root/index.html` directly.

> **One-time setup required:** In the repository **Settings → Pages → Build and deployment**, set the source to **GitHub Actions** to enable deployments.

---

## DesignSprintAgent

This workspace includes a custom GitHub Copilot agent — **DesignSprintAgent** — that guides a Product Owner through the first four phases of a [Google Design Sprint](https://designsprintkit.withgoogle.com/methodology/overview):

| Phase | Focus | Key Activities |
|---|---|---|
| 1 — Understand | Build shared knowledge of the problem space | Sprint Brief, Expert/User Interviews, User Journey Map, HMW Notes |
| 2 — Define | Focus on the highest-impact problem to solve | Cluster HMW Notes, Problem Statement, Sprint Questions, User Persona |
| 3 — Sketch | Generate a wide and diverse set of solutions | Lightning Demos, Crazy 8s, Solution Sketching, Silent Review |
| 4 — Decide | Select the best solution to move forward | Gallery Walk, Heatmap Voting, Speed Critique, Supervote, Storyboard |

### How to Use

1. Open **GitHub Copilot Chat** in this repository.
2. Invoke the agent by typing `@DesignSprintAgent` followed by your message.
3. The agent will ask which phase you are on and guide you from there.
4. All artefacts are automatically saved to the [`design-sprint/`](./design-sprint/) directory.

### Example Prompts

- `@DesignSprintAgent I'm starting a new Design Sprint. Where do I begin?`
- `@DesignSprintAgent I've just finished a user interview. Here's the transcript: [paste transcript]`
- `@DesignSprintAgent I want to run Crazy 8s — is that the right activity for Phase 1?`
- `@DesignSprintAgent We've completed our HMW notes. Can we move to Phase 2?`

### Workspace Structure

See [`design-sprint/README.md`](./design-sprint/README.md) for the full directory layout and phase templates.
