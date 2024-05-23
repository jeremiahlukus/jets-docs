codebuild.fleet_override| nil | Existing Reserved CodeBuild Fleet ARN. This takes precedence over the Jets Managed Fleet created with `codebuild.fleet.enable`. You should only use one or the other.
codebuild.fleet.base_capacity | 1 | The initial number of machines allocated to the compute ﬂeet, which deﬁnes the number of builds that can run in parallel.
codebuild.fleet.enable | false | Enable creation of a Jets Managed Reserved CodeBuild Fleet. Please read for cost considerations: [CodeBuild Fleets]({% link _docs/remote/codebuild/fleet.md %})