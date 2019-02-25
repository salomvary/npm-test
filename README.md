# NPM Continuous Delivery

Usage:

- Any commit to master will be released to npm as a prerelease build (eg. `1.0.4-build.498205821.0`) tagged with `next`.
- Any tagged commit to master will be relased with the exact version to npm tagged with `latest`.
- Releases will only be published from master.

Recommended workflow:

- Make frequent commits to master. Use `npm-test@next` as the "unstable" stream.
- Release stable versions using `npm version patch` (or `minor`, `major`) and `git push origin master --tags`.
