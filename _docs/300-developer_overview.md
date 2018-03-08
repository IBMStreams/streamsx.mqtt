---
title: "Toolkit Development overview"
permalink: /docs/developer/overview/
excerpt: "Contributing to this toolkits development"
last_modified_at: 2018-02-22T12:37:48+01:00
redirect_from:
   - /theme-setup/
sidebar:
   nav: "developerdocs"
---
{% include toc %}
{% include editme %}

For development, the GitFlow branching model is used.

For more information about the Gitflow process, go to this link here:
[Gitflow for Github](https://datasift.github.io/gitflow/GitFlowForGitHub.html)


#### Very brief description

The continuous development is done in the `develop` branch.

*Feature branches* can be used to 
implement features isolated. Feature branches always originate at the `develop` branch and get merged into 
the `develop` branch if a feature is worth to be merged back.

*Release branches* follow the naming convention `release/vX.Y.Z` and originate at the develop branch. They are used to 
prepare a coming release. When a release is ready to be published, a tag is applied. Release branches are merged into 
the `master` and `develop` branch.

*Hotfix branches* originate at a tagged version, for example at the tag `v1.0.0` and follow the naming convention
`hotfix/vX.Y.Z`. They are used to create fixes for released versions, when a a fix cannot be created as new release
starting off from the develop branch. The final release prepared in a hotfix branch is tagged and merged into the `master` 
branch if possible and into `develop` branch.
