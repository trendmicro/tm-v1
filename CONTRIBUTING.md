# Contributing to Trend Vision One OSS projects

Thank you for reading this documentation and considering contributing to our projects. Any contributions that help us improve the platform are valuable and much appreciated, especially if it is meaningful to you or your organization.

Below are several resources and answers to help you understand the projects, where we are heading, and how you can contribute.

Do not hesitate to shoot us an [email](mailto:emailaddress@trendmicro.com) or join us on our [forums](https://success.trendmicro.com/forum/s/topic/0TO4T000000LH90WAG/trend-micro-vision-one). Most articles below introduce our [detailed documentation](https://docs.trendmicro.com/en-us/enterprise/trend-vision-one.aspx).


## Why contribute?

Trend Vision One has an open-source project focused on building platform extensions, connectors, rules, scripts that help our community of customers and partners. If you want to know more about Trend Vision One, you can read the [detailed documentation](https://docs.trendmicro.com/en-us/enterprise/trend-vision-one.aspx) or [request a demo](https://www.trendmicro.com/explore/vision-one-demos).

Whether you are an organization or an individual working or studying cybersecurity and cyber-defense or simply looking for a technical challenge, contributing to the Trend Vision One project may represent a great opportunity.

* You can help grow the community.

* You can adapt the tool to your core interests and work methods by developing features or fixing bugs you are most interested in.


## Where is the project heading?

Now that the project has been released, our goal for the future is two-fold:

* Of course, fixing bugs and developing features identified as non-critical would add to Trend Vision One's power.
* Provide quality open-source enhancements to customers Vision One experiences


## Code of Conduct

Trend Vision One has adopted a Code of Conduct that we expect project participants to adhere to. Please read the [full text](https://github.com/trendmicro/tm-v1/blob/main/CODE_OF_CONDUCT.md) so that you can understand which actions are and are not tolerated.


## How can you contribute?

Any contribution is appreciated, and many don't imply coding. Contributions can range from suggestions for improving documentation, requesting a new feature, reporting a bug, developing features, or fixing bugs yourself.

You can open an issue on the repository with the label "question" for general suggestions or questions about the project or the documentation. We will answer as soon as possible though the formal Trend Micro product supports aren't applied as this OSS project isn't a formal Trend Micro product. If you do not wish to publish on the repository, please see the section below [**"How can you get in touch for other questions?"**](#howcanyougetintouchforotherquestions).

* Just using Trend Vision One's OSS and opening issues if everything is not working as expected will be a huge step forward. See our section about opening an issue. To report a bug, please refer to the [bug reporting module](https://github.com/trendmicro/tm-v1/issues/new?assignees=&labels=&template=bug_report.md&title=). To suggest a new feature, please fill in the feature request [form](https://github.com/trendmicro/tm-v1/issues/new?assignees=&labels=&template=feature_request.md&title=).

* Don't hesitate to flag an issue with the documentation or the templates if you find them incomplete or unclear. You can do that either by opening a [bug report](https://github.com/trendmicro/tm-v1/issues/new?assignees=&labels=&template=bug_report.md&title=) or by sending us a message on our [forums](https://success.trendmicro.com/forum/s/topic/0TO4T000000LH90WAG/trend-micro-vision-one).

* You can look through opened issues and help triage them (ask for more information, suggest workarounds, suggest labels, flag issues, etc.)

* All commits messages must be formatted as: `[component] Message (#issuenumber)` where component should be:
  * API
  * frontend
  * worker
  * doc

### Commit signing requirement

All commits to this repository must be cryptographically signed. This is a firm requirement; unsigned commits cannot be merged regardless of review status.

Signing your commits tells us the code came from who it says it did, which is important for a security-focused project and required by Trend Micro's open-source contribution policy.

Setting up commit signing

GitHub supports two signing methods: GPG keys and SSH keys. Either works.

* GPG signing: [follow GitHub's guide to generating a GPG key and configuring Git to use it](https://docs.github.com/en/authentication/managing-commit-signature-verification/generating-a-new-gpg-key).
* SSH signing: [follow GitHub's guide to signing commits with your SSH key](https://docs.github.com/en/authentication/managing-commit-signature-verification/about-commit-signature-verification#ssh-commit-signature-verification).

Once configured, every commit you make will be signed automatically. You can verify this worked by running:

```bash
git log --show-signature -1
```

If you open a PR and see a message indicating your commits cannot be merged, the most likely cause is unsigned commits. Rebase your branch with signed commits before requesting review:

```bash
git rebase --exec 'git commit --amend --no-edit -S' origin/main
```

### How can you get in touch for other questions?

If you need support or want to discuss the Trend Vision One OSS platform, please join us on our [forums](https://success.trendmicro.com/forum/s/topic/0TO4T000000LH90WAG/trend-micro-vision-one).
