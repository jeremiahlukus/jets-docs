---
title: jets build
reference: true
---

## Usage

    jets build [options]

## Description

Builds and packages project for AWS Lambda

Builds a zip file package to be uploaded to AWS Lambda. This allows you to build the project without deploying and inspect the zip file that gets deployed to AWS Lambda. The package contains:

* your application code
* generated shims

If the application has no Ruby code and only uses Polymorphic functions, then gems are not bundled up.


## Options

```
    [--templates], [--no-templates]  # Build CloudFormation templates only
-e, [--environment=ENVIRONMENT]      # Specifies the environment to run this build under (test/dev/prod).
```

