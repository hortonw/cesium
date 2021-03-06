Thanks for contributing to Cesium.  You rock!  Are you

* [submitting an issue](#submitting-an-issue),
* [getting started contributing](#getting-started-contributing), or
* [opening a pull request](#opening-a-pull-request)?

To ensure an inclusive community, contributors and users in the Cesium community should follow the [code of conduct](#code-of-conduct).

# Submitting an Issue

If you have a question, do not submit an issue; instead, search the [Cesium forum](http://cesiumjs.org/forum.html).  The forum is very active and there are years of informative archives, often with answers from the core Cesium team.  If you do not find an answer to your question, start a new thread and you'll likely get a quick response.

If you think you've found a bug in Cesium, first search the [issues](https://github.com/AnalyticalGraphicsInc/cesium/issues).  If an issue already exists, please add a comment expressing your interest and any additional information.  This helps us prioritize issues.

If a related issue does not exist, submit a new one.  Please be concise and include as much of the following information as is relevant:
* Minimum amount of sample code (and data) shared through [Sandcastle](http://cesiumjs.org/Cesium/Apps/Sandcastle/index.html?src=Hello%20World.html&label=Showcases) using a [GitHub gist](http://cesiumjs.org/2016/04/14/Share-Sandcastle-Examples-Easily-with-GitHub-Gists/).
* Screenshot or animated .gif if appropriate (try [LICEcap](http://www.cockos.com/licecap/)).  For example, see [#3153](https://github.com/AnalyticalGraphicsInc/cesium/issues/3153).  Screenshots are particularly useful for exceptions and rendering artifacts.  If it is a rendering artifact, also include the output of [webglreport.com](http://webglreport.com/).
* Link to the thread if this was discussed on the Cesium forum or elsewhere.  For example, see [#3045](https://github.com/AnalyticalGraphicsInc/cesium/issues/3045).
* Your operating system and version, browser and version, and video card.  Are they all up-to-date?  Is the issue specific to one of them?
* The version of Cesium.  Did this work in a previous version?
* Ideas for how to fix or workaround the issue.  Also mention if you are willing to help fix it.  If so, the Cesium team can often provide guidance and the issue may get fixed more quickly with your help.

# Getting Started Contributing

Everyone is welcome to contribute to Cesium!

In addition to contributing core Cesium code, we appreciate many types of contributions:

* Being active on the [Cesium forum](http://cesiumjs.org/forum.html) by answering questions and providing input on Cesium's direction.
* Showcasing your Cesium apps on the [demos page](http://cesiumjs.org/demos.html) or writing a guest post blog on the [Cesium blog](http://cesiumjs.org/blog.html).  To do either, contact [Sarah Chow](http://cesiumjs.org/team/SarahChow.html), schow@agi.com.
* Writing tutorials, creating examples, and improving the reference documentation.  See the issues labeled [doc](https://github.com/AnalyticalGraphicsInc/cesium/labels/doc).
* Submitting issues as [described above](#submitting-an-issue).
* Triaging issues.  Browse the [issues](https://github.com/AnalyticalGraphicsInc/cesium/issues) and comment on issues that are no longer reproducible or on issues which you have additional information.
* Creating ecosystem projects for [glTF](https://github.com/KhronosGroup/glTF/issues/456), [CZML](https://github.com/AnalyticalGraphicsInc/cesium/wiki/CZML-Guide), and [3D Tiles](https://github.com/AnalyticalGraphicsInc/3d-tiles).

For ideas for Cesium code contributions, see:

* issues labeled [beginner](https://github.com/AnalyticalGraphicsInc/cesium/labels/beginner) and
* issues labeled [roadmap](https://github.com/AnalyticalGraphicsInc/cesium/labels/roadmap).

See the [Build Guide](Documentation/Contributors/BuildGuide/README.md) for how to build and run Cesium on your system.

Always feel free to introduce yourself on the [Cesium forum](http://cesiumjs.org/forum.html) to brainstorm ideas and ask for guidance.

# Opening a Pull Request

We love pull requests.  We strive to promptly review them, provide feedback, and merge.  Interest in Cesium is at an all-time high so the core team is busy.  Following the tips in this guide will help your pull request get merged quickly.

> If you plan to make a major change, please start a new thread on the [Cesium forum](http://cesiumjs.org/forum.html) first.  Pull requests for small features and bug fixes can generally just be opened without discussion on the forum.

## Contributor License Agreement (CLA)

Before we can merge a pull request, we require a signed Contributor License Agreement.  There is a CLA for:

* [individuals](Documentation/Contributors/CLAs/individual-cla-agi-v1.0.txt) and
* [corporations](Documentation/Contributors/CLAs/corporate-cla-agi-v1.0.txt).

This only needs to be completed once.  The CLA ensures you retain copyright to your contributions, and we have the right to use them and incorporate them into Cesium using the [Apache 2.0 License](LICENSE.md).

Please email a completed CLA with all fields filled in to [cla@agi.com](mailto:cla@agi.com).  Related questions are also welcome.

## Pull Request Guidelines

Our code is our lifeblood so maintaining Cesium's high code quality is important to us.

* Review the [Contributor Guides](Documentation/Contributors/README.md).  In addition to Cesium-specific topics, they contain a lot of general software development best practices.
* If this is your first contribution to Cesium, add your name to [CONTRIBUTORS.md](https://github.com/AnalyticalGraphicsInc/cesium/blob/master/CONTRIBUTORS.md).
* For an overview of our workflow see [github pull request workflows](http://cesiumjs.org/2013/10/08/GitHub-Pull-Request-Workflows/).
* Pull request tips
   * If your pull request fixes an existing issue, include a link to the issue in the description (like this: [#1](https://github.com/AnalyticalGraphicsInc/cesium/issues/1)).  Likewise, if your pull request fixes an issue reported on the Cesium forum, include a link to the thread.
   * If your pull request needs additional work, include a [task list](https://github.com/blog/1375%0A-task-lists-in-gfm-issues-pulls-comments).
   * Once you are done making new commits to address feedback, add a comment to the pull request such as `"this is ready"` since GitHub doesn't notify us about commits.
* Code and tests
   * Follow the [Coding Guide](Documentation/Contributors/CodingGuide/README.md).
   * Verify your code passes [ESLint](http://www.eslint.org/).  Run ESLint for all of Cesium with `npm run eslint` or automatically run ESLint when files are saved with `npm run eslint-watch`.  See the [Build Guide](Documentation/Contributors/BuildGuide/README.md).
   * Verify that all tests pass, and write new tests with excellent code coverage for new code.  Follow the [Testing Guide](Documentation/Contributors/TestingGuide/README.md).
   * If you added new identifiers to the Cesium API:
      * Update [CHANGES.md](CHANGES.md).
      * Include reference documentation with code examples.  Follow the [Documentation Guide](Documentation/Contributors/DocumentationGuide/README.md).
      * If the change is significant, add a new [Sandcastle](http://cesiumjs.org/Cesium/Apps/Sandcastle/index.html) example or extend and existing one.
   * If you added third-party libraries, including new version of existing libraries, update [LICENSE.md](LICENSE.md).  Mention it in [CHANGES.md](CHANGES.md).  If you plan to add a third-party library, start a new thread on the [Cesium forum](http://cesiumjs.org/forum.html) first.

# Code of Conduct

One of Cesium's strengths is our community.  Our contributors and users are pushing the 3D geospatial field to amazing new levels.  We rely on an open, friendly, inclusive environment to facilitate this.  As such, we follow the [Contributor Covenant](http://contributor-covenant.org/)'s [Code of Conduct](http://contributor-covenant.org/version/1/4/code_of_conduct.md) to ensure a harassment-free experience in the Cesium community.  Any unacceptable behavior can be confidentially sent to the core team at pcozzi@agi.com.

This applies to the main Cesium repo, forum, twitter, and all channels, including all repos in the [AnalyticalGraphicsInc](https://github.com/AnalyticalGraphicsInc) GitHub organization.
