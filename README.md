# Nextflow Training

## <https://training.nextflow.io>

[![Open in GitHub Codespaces](https://github.com/codespaces/badge.svg)](https://codespaces.new/nextflow-io/training?quickstart=1&ref=master)

<p align="center">
  <a href="https://nextflow.io/">
    <picture>
        <source media="(prefers-color-scheme: dark)" width="350" srcset="https://github.com/seqeralabs/logos/blob/master/nextflow/nextflow_logo_color_darkbg.png?raw=true">
        <img alt="Nextflow Logo" width="350" src="https://github.com/seqeralabs/logos/blob/master/nextflow/nextflow_logo_color.png?raw=true">
    </picture>
  </a>
</p>

Welcome to the Nextflow training repository!
We are excited to have you on the path to writing reproducible and scalable scientific workflows using Nextflow.

- 👉🏻 Written training material: <https://training.nextflow.io>

- 👩🏻‍💻 Instructions on loading this repository within a GitHub Codespaces environment: <https://training.nextflow.io/envsetup/>

- 📚 Nextflow documentation: <https://www.nextflow.io/docs/latest/>

- 💬 Community forum: <https://community.seqera.io/nextflow>

## Contributions

We welcome fixes and improvements from the community. Please fork the repository and create pull-requests with any improvements you'd like to suggest to the docs.

You can find instructions about how to develop the training material code in [`CONTRIBUTING.md`](CONTRIBUTING.md). If you want to contribute with a translation instead, check [`TRANSLATING.md`](TRANSLATING.md).

### Headings CI tests

This repository includes a Python tool to validate markdown heading numbering consistency across training materials.

The `check_headings.py` script ensures:

- Sequential numbering at each level (1., 1.1., 1.2., etc.)
- Trailing periods after heading numbers
- Heading levels match numbering depth (## for 1., ### for 1.1.)

The easiest way to run it is [with `uv`](https://docs.astral.sh/uv/), which handles dependencies for you automatically:

```bash
# Check files for issues
uv run .github/check_headings.py docs/**/*.md
```

```bash
# Auto-fix detected issues
uv run .github/check_headings.py --fix docs/**/*.md
```

Otherwise, run `pip install typer rich` then `python .github/check_headings.py`.

The script runs automatically in CI on markdown file changes via GitHub Actions,
and will cause a CI failure if any incorrect headings are found.

## Credits & Copyright

This training material is developed and maintained by [Seqera](https://seqera.io) and released under an open-source license ([CC BY-NC-ND](https://creativecommons.org/licenses/by-nc-nd/4.0/)) for the benefit of the community. You are welcome to reuse these materials according to the terms of the license. If you are an instructor running your own trainings, we'd love to hear about how it goes and what we could do to make it easier.

<a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/"><img alt="Creative Commons License" src="docs/assets/img/cc_by-nc-nd.svg" /></a>

> Copyright 2025, Seqera. All examples and descriptions are licensed under the <a rel="license" href="http://creativecommons.org/licenses/by-nc-nd/4.0/">Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License</a>.
