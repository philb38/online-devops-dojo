# Online DevOps Dojo  [![License: MPL 2.0](https://img.shields.io/badge/License-MPL%202.0-brightgreen.svg)](https://opensource.org/licenses/MPL-2.0)

This repository contains the source of **Online DevOps Dojo** Katacoda Scenarios
and the coach robot.

In case you are landing here in first place or want to run the trainings, please
first read [about the DevOps Dojo](https://dxc-technology.github.io/about-devops-dojo/).

## Changelog

See a [history of the changes](CHANGELOG.md) to the **Online DevOps Dojo**.

## Files

### Training scenarios

- [`online-devops-dojo-pathway.json`](online-devops-dojo-pathway.json): Index of
Katacoda scenarios
- [`online-devops-dojo/`](online-devops-dojo/): Katacoda scenarios: one sub-folder
for each training
- [`assets/online-devops-dojo/`](assets/online-devops-dojo/): Images used in
training pages

### Dojo coach

- [`docs/`](docs): Some documentation about the coach bot
- [`handler.js`](handler.js): Handler for the Lambda function
- [`index.js`](index.js): Coach code
- [`package.json`](package.json): Node package dependencies
- [`package-lock.json`](package-lock.json): Tested set of Node module dependencies

### Continuous delivery

- [`.github/workflows/upload_lambda.yml`](.github/workflows/upload_lambda.yml):
  GitHub workflow triggered on repository pushes, which upload the coach lambda function.
- [`serverless.yml`](serverless.yml): Serverless deployment configuration file

We have not found a way to isolate the coach files in a sub-folder and execute Serverless
there. Help is welcome.

## Contributing

If you want to contribute to the DevOps trainings, see [the contribution instructions](CONTRIBUTING.md).

If you are interested in the coach, please read its [setup process](docs/bot-setup.md).

## Issues

If you experience some problems with the existing scenarios, please open an
[issue](https://github.com/dxc-technology/online-devops-dojo/issues/new/choose)
and let us know.

## License

This project is licensed under the Mozilla Public License Version 2.0 - see
the [LICENSE](LICENSE) file for details.
