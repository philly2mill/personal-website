# Personal Website — Chris

A basic responsive HTML/CSS website for a class assignment. It includes Home, About, and Hobby pages. Both required pages include bundled stock photographs. No framework, package install, or build step is needed.

## Run locally on macOS

Extract this folder into Downloads. Open Terminal and run:

```bash
cd ~/Downloads/personal-website
python3 -m http.server 8000
```

Open http://localhost:8000 in your browser. Leave Terminal running. Press Control+C to stop the server. If port 8000 is busy, use 8001 and open http://localhost:8001 instead.

## Push to the empty GitHub repository

From a second Terminal window:

```bash
cd ~/Downloads/personal-website
git init
git add .
git commit -m "Build personal website with About and Hobby pages"
git branch -M main
git remote add origin https://github.com/philly2mill/personal-website.git
git push -u origin main
```

These commands assume this extracted folder is not already a Git repository and the remote repository is empty. Authenticate using GitHub's supported sign-in flow if prompted; do not enter an account password as a Git password. If origin already exists, use `git remote -v` to inspect it before changing anything.

## Deploy using GitHub Pages

1. Open the repository on GitHub.
2. Select Settings → Pages.
3. Under Build and deployment, set Source to Deploy from a branch.
4. Select main and /(root), then Save.
5. Wait for the deployment to finish. Use the published URL displayed on the Pages screen.

Expected URL after successful deployment:
https://philly2mill.github.io/personal-website/

Reference: https://docs.github.com/en/pages/getting-started-with-github-pages/configuring-a-publishing-source-for-your-github-pages-site

GitHub Pages serves this static HTML/CSS website. It does not run a Rails or ASP.NET server. The assignment permits GitHub as a deployment option, so Rails is not required unless your professor separately specifies it.

## Verify before submitting

- Open Home, About, and Hobby locally; verify every navigation link.
- Check that both photos display and the layout works at a narrow browser width.
- Repeat those checks at the live GitHub Pages URL.
- Submit the repository URL and live website URL.
- If required, include screenshots of localhost and the live site.

## Photos and customization

The photos are illustrative stock images, not photos of Chris. Both are included locally, so the site does not rely on external image requests.

- images/about.jpg: https://unsplash.com/photos/1516321318423-f06f85e504b3 (image source: https://images.unsplash.com/photo-1516321318423-f06f85e504b3)
- images/running.jpg: image source https://images.unsplash.com/photo-1476480862126-209bfaa8edc8
- Unsplash license: https://unsplash.com/license

If the professor expects a personal photo, replace images/about.jpg with your own JPG and update the alt text and caption in index.html and about.html. You can likewise replace images/running.jpg with a running photo. Keep the filenames or update the HTML paths.

## Problem solution — adapt after you actually deploy

I used GitHub Pages to deploy my website. I built the pages with HTML and CSS and tested them locally using Python's HTTP server. I used Git to commit the website files and push them to my GitHub repository. Then I configured GitHub Pages to publish the main branch from the repository root. After deployment, I checked the public URL to confirm that the About and Hobby pages, navigation, and photos worked.

Only submit that paragraph after completing and verifying those steps.
