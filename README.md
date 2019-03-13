# template-workflow

> A GitHub App built with [Probot](https://github.com/probot/probot) that
> enforces customizable workflow requirements for issues and pull requests.

`template-workflow` requires that your repository have issue or pull request
templates configured. It will only enforce workflow for issues if an issue
template exists and similarly it will only enforce workflow for pull requests if
a pull request template exists.

## Configuration

```yaml
pull_requests:
  field_regex: "\A### (.*)\z"
  required_fields:
    - Code Reviewers
    - Summary of Issue
    - Summary of Change
```

## Setup

```sh
# Install dependencies
npm install

# Run typescript
npm run build

# Run the bot
npm start
```

## Contributing

If you have suggestions for how template-workflow could be improved, or want to report a bug, open an issue! We'd love all and any contributions.

For more, check out the [Contributing Guide](CONTRIBUTING.md).

## License

[ISC](LICENSE) © 2019 Chris Fung <aergonaut@gmail.com>
