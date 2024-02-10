# Work with JSON in BASH using jq

The `jq` command-line tool is is a lightweight and flexible command-line **JSON** processor. It is great for parsing JSON output in BASH.

One of the great things about `jq` is that it is written in portable C, and it has zero runtime dependencies. All you need to do is to download a single binary or use a package manager like apt and install it with a single command.

## Planning the script

For the demo in this tutorial, I would use an external REST API that returns a simple JSON ouput called the [QuizAPI](https://quizapi.io/):

> [https://quizapi.io/](https://quizapi.io/)

If you want to follow along make sure to get a free API key here:

> [https://quizapi.io/clientarea/settings/token](https://quizapi.io/clientarea/settings/token)

The QuizAPI is free for developers.

## Installing jq

There are many ways to install `jq` on your system. One of the most straight forward ways to do so is to use the package manager depending on your OS. 

Here is a list of the commands that you would need to use depending on your OS:

* Install jq on Ubuntu/Debian:

```bash
sudo apt-get install jq
```

* Install jq on Fedora:

```bash
sudo dnf install jq
```

* Install jq on openSUSE:

```bash
sudo zypper install jq
```

- Install jq on Arch:

```bash
sudo pacman -S jq
```

* Installing on Mac with Homebrew:

```bash
brew install jq
```

* Install on Mac with MacPort:

```bash
port install jq
```

If you are using other OS, I would recommend taking a look at the official documentation here for more information:

> [https://stedolan.github.io/jq/download/](https://stedolan.github.io/jq/download/)

Once you have jq installed you can check your current version by running this command:

```bash
jq --version
```