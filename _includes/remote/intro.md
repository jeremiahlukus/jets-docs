Jets uses CodeBuild as the remote runner. CodeBuild provides a consistent build environment, CPU architecture, raw horsepower, and ec2 internet speed. The faster internet speed is particularly useful for pushing Docker images. The CodeBuild project is created as part of `jets deploy` during the bootstrap phase.