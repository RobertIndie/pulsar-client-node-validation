# pulsar-client-node-validation

## Release validation for the pulsar-client-node

* Download the node package corresponding to the environment you are using from the [release candidate link](https://dist.apache.org/repos/dist/dev/pulsar/pulsar-client-node/pulsar-client-node-1.8.0-candidate-1/). (Take 1.8.0-rc1 as the example)
  * Take the example for the macos x64 system: `curl -L -O https://dist.apache.org/repos/dist/dev/pulsar/pulsar-client-node/pulsar-client-node-1.8.0-candidate-1/napi-darwin-unknown-x64.tar.gz`
* Untar the file `tar -xvzf napi-*.tar.gz`
* Start the pulsar standalone from your Pulsar repo or Pulsar environment: `bin/pulsar standalone -nfw -nss`
* Test the loading of the node package: `node ./load_test.js`
* You can also test the examples like producer and consumer:
  * eg. For producer: `node ./examples/producer.js`

