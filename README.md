# .github
Repository for Organisation level:
> - Issue Creation Templates
> - Pull Request Creation Templates

> - Contributing
> - Code of Conduct
> - Funding
> - Security
> - Support

Github configuration information is [here](https://docs.github.com/en/communities/setting-up-your-project-for-healthy-contributions/creating-a-default-community-health-file).

# General
The above list excludes the readme, and the wiki / documentation of the product/project.
It is important that duplication is kept to a minimum, so that these facilities (templates) can and will be kept up to date.

## Readme
The readme is not the contributing, and must not contain anything about contributing other than perhaps a link to contributing.
Similarily, contributing must not discuss things like licencing (Licensing is specific to an individual project and it's dependencies).

Similarily, again;
The readme must introduce the product from a layman and then a developer viewpoint.
Then detail the entire technology stack including the versions used.
If the product/project is some kind of singular tool, then "how to build and run with examples" must be part of the readme when no further documentation is being provided.
If the product/project is not a singular tool, then the instructions belong in documentation, which must be generated from code.

The readme must link to the documentation when documentation is provided.

# Issue Types
> Work
> : Work done that is progress towards a project/product goal, including refactoring AND optimisations (e.g. performance), including more tests.

> Bug
> : Something is not working as intended.

> Security
> : Something is compromised.

> Update
> : Something needs to be updated, including adjusting cloud things.

Isues must address a single issue.

Security has it's own issue type because these should to be added to the product's testing regiment, and it's often more important to very quickly plug the hole than to spend time creating the testing infrastructure that ensures that the hole remains plugged.

Update issues can be created by code-inspection tools, which also means that these need to be managed in a different way than standard work.

There is no feature request issue type, issues are a terrible way to manage feature requests, other tools are specifically built for this kind of decision making.

# Contributing
Contributing must detail the process to be followed before a pull request is created.

In general, the change process should be something like this:
- First discuss in the discussion board for the particular repository the work to be done, unless the work is obvious or already organised.
- Create an issue, of the particular issue type, or nearest best guess issue type.
- Checkout/clone the repository directly, **we do not fork**.
- Ensure that you are on the main branch.
- Ensure that you have the latest main branch locally.
- Ensure that the application runs and that tests pass locally on the main branch.
- If needed, create a ssh key, add the ssh key to your local ssh agent, add the public key to github, request push access to the repository from the repository admin.
- Create a new local branch from main in the format **issue-n**, where n is the issue number.
- Assign the issue to yourself.
- Push your local branch to github (origin). This ensures that only one person is working on an issue at a time, and that the workee can easily be identified.
- Do the work, update the tests, push changes up at any time.
- Update your local main, rebase your work from main and consider squashing it.
- Create the pull request, push the pull request. The pull request text must refer to the issue number. e.g. closes #232.
- Wait patiently.

Do NOT put technical details inside the contributing template. These belong in the readme.
The required test pass/fail ratios and code coverage must be handled automagically, the tools in place must either prevent the creation of a pull request if these have not passed, or the pull request must be tagged as ready-for-review once the requirements have passed.
