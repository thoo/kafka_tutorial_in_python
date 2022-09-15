This tutorial is set up on Mac OS X using `homebrew` installation. In theory, it should work on other platforms.

## Prerequisites
You will need to install `kafka` and `kafka-python` by running the following.
```shell
brew install kafka
pip install kafka_python
```

Then start the service through `homebrew`.
```shell
brew services start zookeeper
brew services start kafka
```

**prducer.ipynb :** This demonstrate how to create a topic, how to set the number of partition and how to send a message through `kafka`.

**consuemr.ipynb :** This demonstrates how to subscribe to a topic. This also displays how the order is preserved within a partition even though it is not guaranteed in a topic.
