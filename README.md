# publish-helm-s3

Github Action to publish helm charts to s3.

Planning on basing this on [this unmaintaned repo](https://github.com/shellbear/helm-release-action) by [shellbear](https://github.com/shellbear) and my [existing in-use fork of it](https://github.com/danielemery/helm-release-action).

This makes use of the [hypoglow helm s3 package](https://github.com/hypnoglow/helm-s3.git).

I'm consider writing it in Rust as a learning experience based on [this blog post](https://dylananthony.com/blog/how-to-write-a-github-action-in-rust/) by [Dylan Anthony](https://dylananthony.com/).

## Goals

- [ ] Achieve feature parity with `helm-release-action`
  - [ ] Allow specifying chart version and chart app version, chart directory and target s3 bucket as action parameters
  - [ ] Deploy chart to s3 bucket with the correct overrides using the hypoglow helm s3 package mentioned above
- [ ] Document full usage examples
- [ ] Publish to github marketplace
- [ ] Link to new terraform module that creates the minimum s3 bucket, IAM user etc for the action to use
- [ ] Write a blog post documenting the motivation, process and package
