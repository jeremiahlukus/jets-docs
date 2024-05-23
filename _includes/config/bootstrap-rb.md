The `bootstrap.rb` has configurations that loaded next for the Jets bootstrap process. The bootstrap phase is the first phase of the Jets deploy process. Example:

config/jets/bootstrap.rb

```ruby
Jets.bootstrap.configure do
  config.codebuild.project.env.vars = {
    BUNDLE_GITHUB__COM: "SSM:/#{ssm_env}/BUNDLE_GITHUB__COM",
    DOCKER_HOST: "SSM:/#{ssm_env}/DOCKER_HOST",
    DOCKER_PASS: "SSM:/#{ssm_env}/DOCKER_PASS",
    DOCKER_USER: "SSM:/#{ssm_env}/DOCKER_USER",
    JETS_SSH_KEY: "SSM:/#{ssm_env}/JETS_SSH_KEY",
    JETS_SSH_KNOWN: "SSM:/#{ssm_env}/JETS_SSH_KNOWN"
  }

  config.codebuild.lambda.enable = true
end
```
