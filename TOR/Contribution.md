# Contributing

Thank you for your interest in contributing to the ETF project. We would
appreciate it if you would read this information carefully so that we can
propagate your changes as soon as possible.

Please read and follow our
[Code of Conduct](https://github.com/guadaltel/governance/blob/8791bedab49372132c2814b95837b4401bfaee5e/CODE_OF_CONDUCT.adoc)
before you interact with the ETF community.

We distinguish between two types of changes to the ETF software
that are handled differently:
- For changes that provide __bug fixes__ a Pull Requests can be created
  that references an existing bug in the
  [ETF webapp](https://github.com/etf-validator/etf-webapp/issues)
  repository.
- Changes that provide __improvements__ to the software must first be
  discussed in an
  [ETF Improvement Proposal (EIP) ](https://github.com/etf-validator/governance/issues/new?template=etf-improvement-proposal--eip-.md)
  and reference an accepted EIP.

Before we can merge you contribution, we must have received you signed
[ETF Entity Contributor License Agreement](https://github.com/etf-validator/governance/blob/c776741d4b1548a7019f55e8873be5c4c1b572c1/CLA/Entity.md).

The ETF project is governed by a
[Steering Group](https://github.com/etf-validator/governance/blob/master/TOR/Steering_Group.adoc)
which is supported by a
[Technical Committee (TC)](https://github.com/etf-validator/governance/blob/master/TOR/Technical_Committee.adoc)
in technical matters. Your Pull Request will be reviewed by the TC.

## Pull Request Process

0. Make sure you have sent us your signed ETF Entity Contributor License Agreement.
   This is only required once.
1. Fork the repository.
2. Create a branch in your forked repository that either references an
   ETF Improvement Proposal (EIP) or an reported bug. The branch name must
   be 'EIP-NUMBER' for an ETF Improvement Proposal, where NUMBER is the
   GitHub issue number from governance repository or 'bug-NUMBER' where
   NUMBER is the GitHub issue number from the ETF webapp repository.
3. Make the code changes. Please also check the Requirements for a Pull Request
   section below.
4. Implement unit tests and test your changes.
   Run all unit tests of the module with the gradle _test_ task.
   Note: your unit tests, additional integration and system tests are
   automatically run by a Continuous Integration system when you create
   the Pull Request and must also be passed.
5. Run the gradle _spottlessApply_ task for an uniform code formatting and for
   ensuring that all Copyright headers are set.
5. Please do not increase the version number. The TC will increase the version
   number for you based on the impact of the change.
7. Push to your branch and then create a Pull Request in our repository.
   Describe your design decisions for new features in the Pull Request.

## Requirements for a Pull Request

1. A Pull Request can be composed by one or multiple commits. All changes
   together address one high-level concern. If a PR provides multiple,
   distinct features from different sections and each section addresses a
   separate concern, without addressing one common high-level concern, it
   will be rejected. Examples for bad PRs: a PR that provides a bugfix and
   adds a feature, a PR that addresses multiple EIPs.
2. Changes must be traceable in the commit history.
2. Make sure you have added Javadocs if you have added public interfaces.
3. Make sure there are no commented out code sections.
4. English language needs to be used in code and comments.
