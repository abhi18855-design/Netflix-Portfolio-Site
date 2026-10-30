# Deploy this portfolio on GitHub Pages

The website's GitHub Actions workflow is already saved at `.github/workflows/deploy.yml`. The leading dot makes `.github` less visible in Finder, but GitHub Actions requires that exact folder and filename. Do not rename it in the repository.

`DEPLOY-WORKFLOW.yml` in this folder is a visible copy for opening and copying. GitHub will not run a workflow from that root-level copy.

## Easiest way to add the workflow through GitHub's website

1. Open `https://github.com/abhi18855-design/Netflix-Portfolio-Site`.
2. Choose **Add file → Create new file**.
3. In the filename box, enter `.github/workflows/deploy.yml`. GitHub will create the folders as you type the slashes.
4. Open `DEPLOY-WORKFLOW.yml` from this local folder, copy all of its text, and paste it into GitHub's editor.
5. Commit the new file to `main`.
6. Under **Settings → Pages**, keep **Source: GitHub Actions**.
7. Open **Actions → Deploy creative portfolio**. If it has not run, choose **Run workflow** on `main`.
8. When the deploy job succeeds, open `https://abhi18855-design.github.io/Netflix-Portfolio-Site/`.

The new portfolio also has a `.pages.yml` file at its root. That hidden file configures the visual content editor. To upload it through GitHub's website, use **Add file → Upload files** and choose `.pages.yml` directly. In Finder, press **Command–Shift–Period** to show dot files. Upload `.pages.yml` to the repository root, not inside another folder.

Avoid uploading `.git`, `node_modules`, or `dist`. The workflow builds `dist` itself from the source files.
