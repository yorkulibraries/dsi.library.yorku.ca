# dsi.library.yorku.ca

This site is built with [Zensical](https://zensical.org). The sections below walk through the most common update tasks.

## How to Update

### Adding New Pages or Editing Existing Pages

1. Create a [fork](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo) or a [branch](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository) of this repository.
2. Work locally on your own machine, or on [GitHub](https://docs.github.com/en/repositories/working-with-files/managing-files/editing-files) editing existing or creating new [Markdown](https://zensical.org/docs/authoring/markdown/) files.
3. [Commit](https://docs.github.com/en/pull-requests/committing-changes-to-your-project) your changes. [Write a good commit message](https://hslguides.med.nyu.edu/c.php?g=1429737&p=10610735). Think of this the way you would document changes or maintain a revision history for an institutional document.
4. Open a [Pull Request](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request) to propose your changes for review.

> **New to Git or GitHub?** The Software Carpentry [Version Control with Git](https://swcarpentry.github.io/git-novice/) course is a solid starting point, including for collaborative workflows.

### Changing Site Structure or Navigation

Navigation is configured in [`zensical.toml`](https://github.com/yorkulibraries/dsi.library.yorku.ca/blob/main/zensical.toml#L40-L78). The nested array in that file controls how the site navigation is organized, and it corresponds directly to how content is structured in the [`docs`](https://github.com/yorkulibraries/dsi.library.yorku.ca/tree/main/docs) folder. Changes to navigation and changes to the `docs` folder structure go hand in hand.

### Working with Images

Store images in the [`docs/images`](https://github.com/yorkulibraries/dsi.library.yorku.ca/tree/main/docs/images) folder. To link to or embed an image anywhere on the site, use the path: `/images/filename.ext`

### ⚠️ Caution: Files to Leave Alone

Unless you have a specific reason and are confident in what you're doing, do not edit or remove the following:

- `.github/workflows`
- `CNAME`
- `docs/stylesheets/extra.css`
