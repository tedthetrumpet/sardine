<h2 align="center">
  <b>Sardine</b>: ✨ Live Coding Library for Python ✨
</h2>
<p align="center"><i>
  Python's missing algorave module. Hackable live coding tool for modern Python (3.10+)
</i></p>

<p align="center">
  <img src=https://img.shields.io/discord/1029399269574193203 />
  <img src=https://img.shields.io/github/license/Bubobubobubobubo/sardine />
  <img src=https://img.shields.io/github/stars/Bubobubobubobubo/sardine />
  <img src=https://img.shields.io/pypi/wheel/sardine-system>
  <img src=https://img.shields.io/pypi/v/sardine-system>
  <img src=https://img.shields.io/pypi/status/sardine-system>
</p>

<p align="center">
  <a href="https://discord.gg/aPgV7mSFZh">Discord</a> |
  <a href="https://sardine.raphaelforment.fr/">Website</a> |
  <a href="https://sardine.raphaelforment.fr/showcase">Examples</a> |
  <a href="https://sardine.raphaelforment.fr/installation/">Installation</a> |
  <a href="https://raphaelforment.fr/">Author</a>  |
  <a href="https://toplap.org/">About Live Coding</a>
  <br><br>
  <p align='center'>
    <a href="https://github.com/bubobubobubobubo/sardine/graphs/contributors">
    <img src="https://contrib.rocks/image?repo=bubobubobubobubo/sardine" />
    </a>
  </p>
</p>

-----------

![Sardine algorave picture](pictures/sardine_intro_picture_repo.png)

**Sardine** is a versatile and hacker-friendly Python library designed for musical improvisation, algorithmic composition, and beyond.
It transforms your standard **Python** interpreter into a powerful music instrument, enabling you to create and map melodic and rhythmic
patterns to any electronic instrument (**MIDI**, **OSC**, and **SuperCollider**).
With **Sardine**, you can:

- **Unleash your musical creativity on stage, in the studio, or for personal enjoyment**
  - Seamlessly communicate with any MIDI/OSC device and the **SuperCollider** audio engine using **Sardine**.
  - Utilize bindings for **SuperDirt**, a widely recognized synthesis engine embraced by live coders globally.

- **Empower your Python code with time-aware capabilities**
  - Employ temporal recursion to make any Python code time and tempo aware.
  - Accurately launch synchronous or asynchronous functions with time-specific results.
  - Customize your own **Senders** or **Receivers** to pattern any desired elements!

- **Develop intricate audio/visual installations with MIDI and OSC *I/O***
  - Assign **callbacks** to any OSC event, transforming **Sardine** into a sophisticated reactive toolbox.
  - Monitor changing values and incorporate them into your musical patterns or code.

- **Synchronize with other computers and musical instruments**
  - Synchronise your hardware with **MIDI Clocks**.
  - Synchronize effortlessly with other tools or players using the **Link Protocol**.

## Installation

In order to install Sardine, your system will require a recent version of Python (3.10+). We now support 3.11 versions as well.
A more detailed installation guide can be found on [Sardine's website](https://sardine.raphaelforment.fr/technical/installation/).
Refer to the website for complete details concerning the installation process.

1) Run: `python -m pip install --find-links https://thegamecracks.github.io/python-rtmidi-wheels/ sardine-system`.
    - the `--find-links` option is used as a temporary fix to the unavailability of some dependencies in the Pypi repositories for Python 3.10/3.11.
2) Install [SuperCollider](https://supercollider.github.io/) and [SuperDirt](https://github.com/musikinformatik/SuperDirt) for an additional supported audio backend.
3) Run `sardine-config` and configure Sardine to your liking following [this guide](https://sardine.raphaelforment.fr/configuration.html)
4) Install the text editor of your choice: VSCode, Neovim, Vim, Emacs, Jupyter Notebook, etc... There are many options you can pick from. They have all been tested with Sardine.

## Contributions

Sardine is in its early stages of development, and we're actively seeking contributors to help enhance the project. If you're passionate
about music and technology, we welcome your expertise, whether it's code, documentation, or ideas. We are looking for contributors! 

To collaborate with the Sardine community, connect with us on **Discord**, **Github** or send a private message if you have specific inquiries.
Together, we can create an even more powerful tool for musical expression and creativity!

## Experimental Bash Script

In the sardine directory, you will find a script called `install_sardine.sh`. This script automates the installation process for you.
Depending on your platform, follow the instructions below to run the script:

### macOS and Linux

1) Open a terminal and navigate to the `sardine` directory.
2) Make the script executable by running: `chmod +x install_sardine.sh`
3) Execute the script: `./install_sardine.sh`

### Windows

The script will taunt you to install most of the dependencies manually. The installation can't really be automated on Windows.

1) Install [Git for Windows](https://git-scm.com/download/win) if you haven't already.
2) Open Git Bash and navigate to the sardine directory.
3) Execute the script: `bash install_sardine.sh`

The script will try (**and fail**) to install the required dependencies and set up the environment for you. It will:

- Install [Git](https://git-scm.com/), [NPM](https://www.npmjs.com/), and [Yarn](https://yarnpkg.com/) (if not already installed)
- Install and configure `pyenv` with Python 3.11 ([PyEnv](https://github.com/pyenv/pyenv))
- Install the Sardine package
- Install `SuperCollider` and [SuperDirt](https://github.com/musikinformatik/SuperDirt) Quarks
- Please be patient, as this process may take some time.
