# Setup guide — Krish Sahu's GitHub profile

## What is included?

- `README.md`: the profile content to use in the special repository named exactly `krish-23CH10035`.
- `assets/hero.gif`: custom animated banner, personalized with the headshot you uploaded.
- `assets/architecture.gif`: custom animated technology-flow diagram.
- `.github/workflows/snake.yml`: optional GitHub Actions workflow that creates a contribution-snake SVG and publishes it to an `output` branch.

## Put the profile online

1. Open `https://github.com/krish-23CH10035/krish-23CH10035`. This special repository must have the same name as your GitHub username. If it already exists, back it up first.
2. Upload/replace `README.md` and the full `assets` folder. Keep the folder structure intact; the README references images by relative path.
3. Copy `.github/workflows/snake.yml` into the same repository at `.github/workflows/snake.yml`.
4. Commit the changes. The README, banner, and architecture GIF should appear on your GitHub profile.

## What is GitHub Actions?

GitHub Actions is GitHub's built-in automation runner. A workflow is a recipe written in YAML that GitHub runs on its hosted computers. This workflow asks an open-source tool to read the public contribution calendar, generate two SVG snake animations, then publish those generated files to a branch called `output`. The README embeds one of those SVGs.

You do **not** need to install anything locally or create a personal access token for this workflow. It uses the repository's built-in `GITHUB_TOKEN`.

## Enable the contribution snake

1. Open the profile repository's **Settings → Actions → General**.
2. Under **Workflow permissions**, select **Read and write permissions** if repository policy requires it; save the setting.
3. Open the **Actions** tab, choose **Generate contribution snake**, and click **Run workflow**.
4. Wait for the run to succeed. It creates an `output` branch containing the snake SVGs. The snake image in the profile README may remain broken until this first successful run.
5. Future runs are scheduled daily. You can also run the workflow manually from the Actions tab.

## Before publishing — a few checks

- Confirm the NovaMind AI repository URL. Your CV describes NovaMind AI, but its repository URL was not included in the links provided, so the README intentionally does not guess it.
- Confirm that the QuickAI repository is the project you want to showcase under that name; the description is deliberately generic until its README/code is checked.
- Keep any internship code, internal company URLs, customer data, credentials, and proprietary screenshots out of public repositories.
- The GitHub stats, streak card, and skill icons use external image services. If one becomes unavailable, remove or replace that image line; the main README and custom GIFs still work.
- The profile uses your uploaded photo inside the banner. Replace `assets/hero.gif` with a version without the portrait if you prefer not to display it publicly.

## Useful links

- Profile repository: https://github.com/krish-23CH10035/krish-23CH10035
- GitHub profile: https://github.com/krish-23CH10035
- Contribution-snake generator: https://github.com/Platane/snk
