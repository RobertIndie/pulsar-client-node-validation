# pulsar-client-node-validation

## Release validation for the pulsar-client-node

* Run `npm install`.
* Start the pulsar standalone from your Pulsar repo or Pulsar environment: `bin/pulsar standalone -nfw -nss`
* Test the loading of the node package: `node ./load_test.js`
* You can also test the examples like producer and consumer:
  * eg. For producer: `node ./examples/producer.js`

## Release validation on GitHub Actions

* Create an issue and paste the package name and version for the release candidate(eg. `pulsar-client@1.8.0-rc.2`) to the issue body.
* Check `GitHub Actions`, it will automatically trigger the validation for multiple platforms. But currently, the validation on the macOS arm64 platform cannot be done in the CI.

