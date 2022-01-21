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
