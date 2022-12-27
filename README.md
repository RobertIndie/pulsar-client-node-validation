# pulsar-client-node-validation

## Release validation for the pulsar-client-node

* Run `npm install`.
* Start the pulsar standalone from your Pulsar repo or Pulsar environment: `bin/pulsar standalone -nfw -nss`
* Test the loading of the node package: `node ./load_test.js`
* You can also test the examples like producer and consumer:
  * eg. For producer: `node ./examples/producer.js`

## Release validation on GitHub Actions
![](https://github.com/RobertIndie/pulsar-client-node-validation/actions/workflows/ci-release-validation.yml/badge.svg)

There is a workflow to run the release validation on multiple platforms. But currently, the validation on the macOS arm64 platform cannot be done in the CI.
