# How to release

- Create a pr to upgrade `Cargo.toml` `package.version` version and merge this pr to master.
- Create a tag(must start with `v` char) based on master branch and push to origin.
    - git checkout master
    - git pull
    - git tag vx.y.z
    - git push origin vx.y.z
- After above steps, the release workflow will be triggered and create a new release in `Github release` and a new package
  in [crates](https://crates.io/search?q=sn-pulsar)