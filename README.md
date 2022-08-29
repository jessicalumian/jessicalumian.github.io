# Blog repo

Blog repository. Theme from [al-folio](https://github.com/alshedivat/al-folio).

### Workflow

Make changes in main branch from command line in markdown files. Push changes.

Then, deploy changes. In root of repo, run:

```
./bin/deploy
```

Then answer yes. This will push changes from the markdown in main branch to gh-pages branch, which is set host the built site.
