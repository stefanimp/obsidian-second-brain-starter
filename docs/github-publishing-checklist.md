# GitHub Publishing Checklist

## Before Creating the Repository

- [ ] Review all files for private names, personal links, local paths, and private context.
- [ ] Decide repository visibility: public.
- [ ] Recommended name: `obsidian-second-brain-starter`.
- [ ] Recommended description: `A clean Obsidian starter kit for building a practical second brain with MOCs, properties, templates, and review workflows.`
- [ ] Add topics: `obsidian`, `pkm`, `second-brain`, `markdown`, `dataview`, `note-taking`, `templates`.

## First Commit

Suggested commands from inside the repository folder:

```bash
git init
git add .
git commit -m "Initial Obsidian second brain starter kit"
```

## Create GitHub Repository

With GitHub CLI:

```bash
gh repo create obsidian-second-brain-starter --public --source=. --remote=origin --push
```

Or create the repository manually on GitHub and then run:

```bash
git remote add origin https://github.com/<username>/obsidian-second-brain-starter.git
git branch -M main
git push -u origin main
```

## After Publishing

- [ ] Add the GitHub link to the LinkedIn article.
- [ ] Add the article link to the GitHub README.
- [ ] Pin the repository on GitHub.
- [ ] Add the repository to LinkedIn Featured.
- [ ] Keep issues enabled if you want feedback.
- [ ] Add screenshots later only if they are generated from the public starter kit, not from the private vault.
