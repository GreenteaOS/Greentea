### Nightly builds and CI

#### What is CI and nightly build?

Continuous Integration - methodology of regular rebuild and testing directly during the development process.
Almost every change is built and tested. Thus, it makes it possible to have an early response about the quality of the product.

#### When does the build take place?

* When a developer makes changes to the GreenteaOS/Kernel repository
* When the contributor sends a request to merge changes (Pull Request)
* When the contributor makes commits to his pull request

#### Where can I see the build status?

* When you request a merge in the `Conversation` tab, below you can see a fairly bright status of `Build` in
yellow (in progress), red (the build failed or contains errors) and green (build successful) colors.
* You may find the link to the build log at top right corner
* Not to be confused with the status of merge possibility!
* Follow the link https://ci.appveyor.com/project/PeyTy/kernel-vwmh6

#### Where to download a build?

Go to the website of the CI system, select the build of interest, and click on the Artifacts tab.

Official GreenteaOS/Kernel nightly builds take place here https://ci.appveyor.com/project/PeyTy/kernel-vwmh6/build/artifacts
