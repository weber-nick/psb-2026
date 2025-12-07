## Creating a New GitHub Repository and Publishing

1. Go to [github.com](https://github.com) and log in.
2. Click the **+** icon (top right) and select **New repository**.
3. Name your repository `nih-psb-2026` and set it to public (or private if preferred).
4. Do NOT initialize with a README, .gitignore, or license (these files already exist locally).
5. Click **Create repository**.
6. In your terminal, run the following commands:
	```sh
	git init
	git remote add origin https://github.com/<your-github-username>/nih-psb-2026.git
	git add .
	git commit -m "Initial site setup"
	git branch -M main
	git push -u origin main
	```
	Replace `<your-github-username>` with your actual GitHub username.
7. Go to your repository on GitHub, then follow the Publishing to GitHub Pages instructions above.
# nih-psb-2026

This repository contains the static website for the NIH workshop at the Pacific Symposium on Biocomputing (PSB) 2026, led by O. Ramwala, N. Weber, and S. Mooney. The site is built with Jekyll for easy editing in Markdown and is intended for publication via GitHub Pages.

## About the Conference

The Pacific Symposium on Biocomputing (PSB) is an international, multidisciplinary conference for the presentation and discussion of current research in the theory and application of computational methods in problems of biological significance. For more information, visit [psb.stanford.edu](https://psb.stanford.edu).

## NIH Workshop

This workshop, organized by Ramwala, Weber, and Mooney, focuses on advancing computational approaches in biomedical research, fostering collaboration, and sharing innovative solutions to pressing challenges in the field.

## Editing & Contribution

- All content is written in Markdown for simplicity.
- To contribute, edit the Markdown files and submit a pull request.
- For setup instructions, see below.

## Setup Instructions

1. Ensure you have Ruby and Bundler installed.
2. Install Jekyll dependencies: `bundle install`
3. Serve locally: `bundle exec jekyll serve`
4. Visit `http://localhost:4000` to preview.

## Publishing to GitHub Pages

1. Commit all your changes:
	```sh
	git add .
	git commit -m "Update site content"
	git push origin main
	```
2. Go to your repository on GitHub.
3. Click **Settings** > **Pages**.
4. Under "Source," select the branch (usually `main`) and `/ (root)` folder.
5. Save and wait for GitHub Pages to build and deploy your site.
6. Your site will be available at `https://<your-github-username>.github.io/nih-psb-2026` (replace with your username).

**Note:** GitHub Pages will automatically build your site using Jekyll. You do not need to build locally unless you want to preview changes before publishing.

## License

This project is open source under the MIT License.
