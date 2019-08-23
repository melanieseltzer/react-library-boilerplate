## Sending a Pull Request

- Find or open a new issue in the [Issue tracker](https://github.com/githubName/repoName/issues).
- Fork the repo and follow these steps to get it running locally:

```bash
$ git clone <library-name>
$ cd <library-name>
$ yarn link
$ yarn install
$ yarn start
```

Add a `.env` file in the root of the example dir and add the following:

```
SKIP_PREFLIGHT_CHECK=true
```

In a new terminal tab:

```bash
$ cd example
$ yarn link "<library-name>"
$ yarn install
$ yarn start
```

Both the library dir and the example dir will watch for changes and rebuild, so whenever you make a change to the library, the example will get it.

- Create a new feature branch based off the `master` branch.
- Do your work 😄
- Submit a pull request, referencing any issues it addresses.

Please try to keep your pull request focused in scope and avoid including unrelated commits.

Thank you for contributing!
