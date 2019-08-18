# Contributing to node-updown

This package welcomes contributions of any kind.

## Process
How to contribute:

1. Open an issue to discuss the changes you want to make
2. Fork the project and implement the changes in your fork
3. Update the readme, tests and any other necessary related files
4. Create a pull request with the changes
5. The pull request will be reviewed by a contributor
6. Your contribution will be merged once the pull request is reviewed and no further changes are necessary

## Code of conduct
I don't want to make a big deal about this. Be friendly, use common sense and remember that we're all humans.

## Style guides

### Formatting
This project contains an `.editorconfig` file, which dictates several basic settings for your IDE. See [editorconfig.org](https://editorconfig.org/#download) to find a plugin for your IDE of choice.

### Code style
The library and tests are written entirely in Typescript. The code is linted by ESLint, so you can see the `.eslintrc.js` file for more information on the exact ruleset used. You can also look at the existing files and follow the same formatting.

If there are questions about the code style, feel free to open an issue.

### Tests
To run the tests, create a `.env` file in the project root and add two values to it:

```
UPDOWN_API_KEY=[your key here]
UPDOWN_READONLY_API_KEY=[your readonly key here]
```

You can also add these to your environment variables manually when running the tests. 

The tests are written for a test account with some dummy data so all API endpoints return some data. Specifically, the tests expect 1 check to exist with at least one previous downtime and at least one successful check having been executed.

__Warning__: These are your personal API credentials, so take good care not to commit this file to the repository or publish it anywhere.