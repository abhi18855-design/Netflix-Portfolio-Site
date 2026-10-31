# Your web editor

The editor is saved in your site folder as `public/editor.html`.

1. In your GitHub repository, open the `public` folder.
2. Choose **Add file → Upload files** and upload `editor.html` into that folder.
3. Ensure the repository root contains `.pages.yml` (starting with a dot). If it still contains only `pages.yml`, rename that file on GitHub. The site build requires the dotted filename.
4. Commit and wait for the GitHub Actions deployment to succeed.
5. Open https://abhi18855-design.github.io/Netflix-Portfolio-Site/editor.html

The editor URL becomes available only after a successful deployment. Uploading the file to the repository root will not work with this Astro build; it belongs inside `public`.

## Edit and publish

- Edit site/contact details, About content, projects, categories, gallery images, audio, and links. Add media under **Media uploads**, then copy its displayed path into the relevant content field.
- New projects begin unpublished. Turn on **Published** when ready. Turn it off to remove a project from the live site without needing to delete files on GitHub.
- Use **Save editing backup** before closing the tab. Use **Open backup** to resume later. Changes are not automatically saved to your computer or GitHub.
- Click **Download updated site ZIP**. Extract the ZIP and upload its contents into the repository root, preserving folders. Do not upload the ZIP itself or a containing folder.
- On Mac, press **Command + Shift + .** to reveal hidden files. Include `.pages.yml` and `.github/workflows/deploy.yml`. Keep existing hidden deployment files when uploading updates.
- Commit the upload, wait for Actions to succeed, then refresh the site and editor. The ZIP contains a refreshed editor with your latest content.

The editor has no GitHub login or publishing permissions. Anyone with its public URL can make their own downloadable copy, but only someone with repository write access can publish changes. Like your public repository, the editor includes project source and draft content. Do not put secrets in it.

This is a content editor with an accent-colour setting, not a drag-and-drop layout designer. It does not render a live site preview. GitHub's browser upload limit is 25 MB per file; because the editor embeds its media, the editor file itself can reach that limit as the library grows. For larger collections, use GitHub Desktop or Git rather than browser uploads.
