# Important - Read Carefully!

Before you submit an issue for Sails, please make sure you have [read the issue contribution guide](https://github.com/balderdashy/sails/blob/master/CONTRIBUTING.md#ii-issue-contributions) carefully, and then verify the following:

- [ ] I am experiencing a concrete technical issue with Sails (ideas and feature proposals should follow the [guide for proposing features and enhancements](https://github.com/balderdashy/sails/blob/master/CONTRIBUTING.md#v-proposing-features-and-enhancements), which involves making a pull request).
- [ ] I am not asking a question about how to use Sails (please refer to the [documentation](http://sailsjs.org), or post on [StackOverflow](http://stackoverflow.org), our [Google Group](https://groups.google.com/forum/#!forum/sailsjs) or our [live chat](https://gitter.im/balderdashy/sails?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)).
- [ ] I have already searched for related issues, and found none open (if you found a related _closed_ issue, please link to it in your post).
- [ ] I am reporting _one_ issue in my post (multiple unrelated issues should be reported in multiple posts).
- [ ] My issue title is concise, on-topic and polite ("jst.js being removed from layout.ejs on lift" is good; "templates dont work" or "why is sails dumb" are not so good).
- [ ] I have tried all the following (if relevant) and my issue remains:

  - [ ] Make sure you have the right app lifted.
  - [ ] Make sure you've killed the Sails server with CTRL+C and started it again.
  - [ ] Make sure you closed any open browser tabs pointed at localhost before starting Sails.
  - [ ] Make sure you do not have any other Sails apps running in other terminal windows.
  - [ ] Make sure the app you are using to reproduce the issue has a clean node_modules/ directory, meaning:
    * no dependencies are linked (e.g. you haven't run npm link foo)
    * that you haven't made any inline changes to files in the node_modules/ folder
    * that you don't have any weird global dependency loops The easiest way to double-check any of the above, if you aren't sure, is to run: rm -rf node_modules && npm cache clear && npm install.
- [ ] I am including my Sails version, Node version, NPM version and operating system in my issue post
- [ ] If I am using the _master_ (development) branch of Sails, I have verified that my issue also exists with the most recent published Sails version (we welcome bug reports against code under development, we just ask that you also verify that this is a _new_ issue versus something that also exists in the published version of Sails).

and finally...
- [ ] **I can provide steps to reproduce this issue that others can follow.**

Ideally, this involves creating a new repo that demonstrates the problem (see instructions [here](https://gist.github.com/sgress454/76be129ebcf07beb203f)).  Even though your issue may seem so simple to reproduce that a new repo is unnecessary, you'd be surprised how many solutions present themselves when you start from `sails new` and attempt to recreate your issue from scratch in a new app.  This ensures that the real issue isn't in your user code (a forgotten [policy file](http://sailsjs.org/documentation/concepts/policies), perhaps?) or in a third-party module.  If you're absolutely _convinced_ that a new repo is unnecessary, provide clear, concise and _specific_ steps to reproduce the problem in your post (not "create a model then do blueprint create").

**To prove that you've read this document carefully** and verified that your issue meets the criteria for a new post, please put `[issue]` in your post title, e.g. `[issue] Error when using layouts with Handlebars templates`.  Posts without `[issue]` in the title will receive a firm warning from [Sailsbot](https://twitter.com/sailsbot) and may be closed.

:heart: the Sails core team.
