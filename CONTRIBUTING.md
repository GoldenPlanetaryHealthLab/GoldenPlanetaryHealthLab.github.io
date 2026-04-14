# Contributing

We welcome contributions to the Golden Lab Data Science Handbook! If you have suggestions for improvements, additional content, or corrections, please feel free to submit a pull request or open an issue on our GitHub repository.

## `all-contributors` Specification

We use the `all-contributors` specification to recognize and celebrate the contributions of everyone 
who has helped with this project. This includes not only code contributions but also 
documentation, design, and other forms of support e.g. feedback, issue submission and conversation, etc.

You can automate the process of adding contributors by using the `all-contributors` 
CLI tool. On Mac, install `npm` first:

```bash
brew install npm node
```

Then, use the following command to add a contributor:

```bash
npm install all-contributors-cli
```

The project is already initialized with `all-contributors`, so you can start adding contributors right away.
You can add contributors from the command line. For example, to add a contributor with 
the username `octocat` who has contributed code and documentation, you would run:

```bash
npx all-contributors add octocat code,doc
```

And then create the contribution table with:

```bash
npx all-contributors generate
```

This will update the `README.md` file with the new contributor and their contributions. Commit
and push this file to GitHub to see the changes reflected in the repository's README.
