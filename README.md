# ipyaladin

A bridge between Jupyter and Aladin Lite, enabling interactive sky visualization in IPython notebooks.
With a couple of lines, you can display Aladin Lite, center it on the target of your choice, and overlay an Astropy table:

![ipyaladin example](assets/ipyaladin-screencast.gif)

- [ipyaladin](#ipyaladin)
  - [Examples](#examples)
  - [Installation](#installation)
  - [Development installation](#development-installation)
  - [How does it work?](#how-does-it-work)

## Examples

Some example notebooks can be found in the [examples directory](examples).

[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/cds-astro/ipyaladin/master). You can also try it directly [in mybinder](https://mybinder.org/v2/gh/cds-astro/ipyaladin/master), without installing anything.

## Installation

To install use pip or conda :

```shell
> pip install ipyaladin
```

You can already try to load ipyaladin in a notebook.

```python
from ipyaladin import Aladin
aladin = Aladin()
aladin
```

## Development installation

First, make sure you have installed jupyter in your python environnement: `pip install jupyter`.
For a development installation [Node.js](https://nodejs.org) and [Yarn version 1](https://classic.yarnpkg.com/) are also required,

```shell
> git clone https://github.com/cds-astro/ipyaladin.git
> cd ipyaladin
> npm install
> npm run dev
```

And you are ready to develop! Any change done in the python, javascript, or css files should
be directly reflected in the notebook editor of your choice (JupyterLab, VSCode,...)!

## How does it work?

Ipyaladin brings [Aladin-lite](https://github.com/cds-astro/aladin-lite) into notebooks thanks to
[Anywidget](https://anywidget.dev/).

Correspondence table between ipyaladin versions and Aladin-lite versions:

| ipyaladin  | Aladin-Lite |
| ---------- | ----------- |
| 0.3.0      | 3.3.3-dev   |
| unreleased | 3.4.1-beta  |
