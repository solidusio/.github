## Releasing a new version

_Requires permission to both push to the master/main branch and to rubygems._

1. Ensure that the CI is green
2. Update the version in `lib/solidus_extension_name/version.rb`
3. Commit the changes with the message `Release vX.Y.Z`
4. Run `bin/rake release` (this will build, create the git tag, and push to both git and rubygems)
5. [Create the GitHub release](https://docs.github.com/en/repositories/releasing-projects-on-github/managing-releases-in-a-repository#creating-a-release) and [auto-generate the changelog](https://docs.github.com/en/repositories/releasing-projects-on-github/automatically-generated-release-notes)
