# Work with JSON in BASH using jq

The `jq` command-line tool is is a lightweight and flexible command-line **JSON** processor. It is great for parsing JSON output in BASH.

One of the great things about `jq` is that it is written in portable C, and it has zero runtime dependencies. All you need to do is to download a single binary or use a package manager like apt and install it with a single command.

## Planning the script

For the demo in this tutorial, I would use an external REST API that returns a simple JSON ouput called the [QuizAPI](https://quizapi.io/):

> [https://quizapi.io/](https://quizapi.io/)

If you want to follow along make sure to get a free API key here:

> [https://quizapi.io/clientarea/settings/token](https://quizapi.io/clientarea/settings/token)

The QuizAPI is free for developers.