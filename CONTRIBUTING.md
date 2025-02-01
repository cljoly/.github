<!-- insert
---
title: "Contribution Guidelines"
date: 2021-10-02T21:00:23+02:00
weight: 2000
draft: false
aliases:
  - "/docs/contribute"
---

{{< rawhtml >}}
<div class="badges">
{{< /rawhtml >}}
end_insert -->

[![Git Email](https://img.shields.io/badge/Git_email-supported-success?style=flat)](#i-dont-want-to-use-github)
[![Contributions welcome!](https://img.shields.io/badge/Contributions_welcome!-3DA639?style=flat)](#tldr)
[![Contributor Covenant](https://img.shields.io/badge/Code_of_conduct-4baaaa.svg?style=flat)][coc]
[![Security Policy](https://img.shields.io/badge/Security_policy-purple.svg?style=flat)][sp]
[![Buy me a tea](https://img.shields.io/badge/Buy_me_a_tea-F96854?style=flat)][tea]

<!-- insert
{{< rawhtml >}}
</div>
{{< /rawhtml >}}
end_insert -->

Thanks for considering contributing! [My projects][oss] all follow the guidelines outlined in this document.

## TL;DR

If you just want to fix a typo or another very small thing, just create a PR.

## Documentation

As the author of a tool or library, we are blind to many of the problems that users may encounter. As an external person, you have the power to spot this! Feel free to open an issue or to send a PR with proposed changes to the documentation.

## Code

### Pull Request

* It is advisable, **but not mandatory**, to create an issue to discuss the feature you want to add, so that you can make sure it has good chances to be merged. This also avoids having multiple persons working on the same thing.
  * Similarly, feel free to create a [draft PR][draft] with your changes before they are completed. This is useful to point to a particular part of the code during discussions.
* Try to create one pull request per high level feature or bug fix. Then if necessary [try to stage your changes][stage] by crafting multiple commits: if your commits follow a progression on your changes, it’ll be easier to review.
* New features need to be covered by adding new unit tests, where applicable. Similarly, bug fixes need to be accompanied by a regression test where applicable, to ensure that the bug does not come back. Reviewers and maintainers are in charge of enforcing this.

### I Don’t Want to Use GitHub

That’s fine, feel free to send your contributions [by email][email][^am] to the address listed [on the Contact page][contact].

If you are contributing this way, please use the [`-s`/`--signoff`][signoff] with each commit, so that a `Signed-off-by` trailer is added to each of your commits.
Or manually add a `Signed-off-by` trailer at the end of your commits, like this:
```
Signed-off-by: Put Your Name Here <TheEmailYou@UseWith.Git>
```
This signifies your agreement with the [DCO below][dco-section].

### I Don’t Know What to Do

If you don’t know what to do, but still want to help, that’s great! Look for issues labeled [`good-first-issue`][gh-first] or [`help-wanted`][gh-help]. You can also [contact me][contact], and tell me about your interests and skills.

### Dependencies

As much as possible, I limit the number of dependencies used in my projects. Dependencies provide a short term win, by relying on someone else’s expertise and implementation to solve a particular problem. But there are two main long-term costs:
1. [ongoing maintenance][build_it_yourself], where one has to spend more and more time just updating an ever expanding tree of dependencies.
1. security risks: both in terms of making sure every dependency and transitive dependency is not a malware in disguise, especially as the authors change.

Please avoid introducing new dependencies in your PRs if possible. If you do, please outline why you think it’s a worthy trade off.

## Delegating Trust

In light of the [XZ-backdoor][xz-backdoor] and many other [supply-chain attacks][supply-chain], I can’t give commit permissions lightly.

As a result I don’t delegate commit rights unless:
1. I’ve known someone in person for years, **and**
2. they have established a track-record of contributions.

It may mean that a project goes abandoned or doesn’t improve as quickly.
Or that it may be overtaken by a fork that gets more attention.
That’s fine.
It’s the trade off I make.
I would rather a fork succeed than letting [a nefarious actor inherit the trust I’ve built][oss-interactions].

## Hobby Project: Take It Slow

My projects are hobby projects.
They are done during my, and contributor’s, free time.
It may mean that your comments or PR may go unanswered for days or weeks.
I value comments, PRs and otherwise constructive interactions.
It’s part of the joy of working on Open-Source software for me.
But I may not have bandwidth to review some changes in a timely manner.
I’m not a full-time Open-Source maintainer.
At least, not yet.
That’s life.

Equally, as a contributor, please feel free to say that you don’t have time or energy anymore.
You can do that even in the middle of a PR.
Someone else can always pick it up.

We are here to have fun developing software.
We don’t owe anything[^try] to consumers of our software.
After all, our Open-Source licenses disclaim as much.

## Code of Conduct

To foster a welcoming environment, we also follow and enforce [a code of conduct][coc].

## Meaning of “Signed-off-by” Lines in Commit Messages

When `Signed-off-by` trailers are used, it means that the committer agrees to the representations from [the Developer Certificate of Origin (DCO)][DCO], reproduced below:

```
Developer's Certificate of Origin 1.1

By making a contribution to this project, I certify that:

(a) The contribution was created in whole or in part by me and I
    have the right to submit it under the open source license
    indicated in the file; or

(b) The contribution is based upon previous work that, to the best
    of my knowledge, is covered under an appropriate open source
    license and I have the right under that license to submit that
    work with modifications, whether created in whole or in part
    by me, under the same open source license (unless I am
    permitted to submit under a different license), as indicated
    in the file; or

(c) The contribution was provided directly to me by some other
    person who certified (a), (b) or (c) and I have not modified
    it.

(d) I understand and agree that this project and the contribution
    are public and that a record of the contribution (including all
    personal information I submit with it, including my sign-off) is
    maintained indefinitely and may be redistributed consistent with
    this project or the open source license(s) involved.
```

This is the DCO used by the Linux kernel and Git projects.

When a `Signed-off-by` trailer is *not* present, we are relying on any provisions of the project’s license.
In addition, if the contribution was submitted through GitHub, the GitHub Terms of Service apply, in particular [Section D.6][gh-terms-d6] ([archived version][gh-terms-d6-archive]).


> 6. Contributions Under Repository License
>
> Whenever you add Content to a repository containing notice of a license, you license that Content under the same terms, and you agree that you have the right to license that Content under those terms. If you have a separate agreement to license that Content under different terms, such as a contributor license agreement, that agreement will supersede.
>
> [...]

## See Also

The other [Open-Source documents][docs].

[^try]: I do try to produce high-quality, secure software. I take pride in my work. But there is no guarantee. That’s the bargain in volunteer-maintained Open-Source software.
[^am]: If you want to accept patches by email too, [git-am.io][git-am] is a good starting point.

[DCO]: https://developercertificate.org
[dco-section]: #meaning-of-signed-off-by-lines-in-commit-messages
[coc]: https://cj.rs/docs/code-of-conduct/
[contact]: https://cj.rs/contact
[docs]: https://cj.rs/open-source/docs/
[draft]: https://github.blog/2019-02-14-introducing-draft-pull-requests/
[email]: https://git-send-email.io/
[gh-first]: https://github.com/search?q=user%3Acljoly+label%3A%22good+first+issue%22+state%3Aopen&type=Issues
[gh-help]: https://github.com/search?q=user%3Acljoly+label%3A%22help+wanted%22+state%3Aopen&type=Issues
[gh-terms-d6-archive]: https://web.archive.org/web/20240817042952/https://docs.github.com/en/site-policy/github-terms/github-terms-of-service#6-contributions-under-repository-license
[gh-terms-d6]: https://docs.github.com/en/site-policy/github-terms/github-terms-of-service#6-contributions-under-repository-license
[git-am]: https://git-am.io/
[oss-interactions]: https://robmensching.com/blog/posts/2024/03/30/a-microcosm-of-the-interactions-in-open-source-projects/
[oss]: https://cj.rs/open-source
[sp]: https://cj.rs/docs/security/
[stage]: https://github.blog/2022-06-30-write-better-commits-build-better-projects/#structure-the-narrative
[supply-chain]: https://en.wikipedia.org/wiki/Supply_chain_attack
[tea]: https://cj.rs/donate
[xz-backdoor]: https://security.archlinux.org/CVE-2024-3094
[build_it_yourself]: https://lucumr.pocoo.org/2025/1/24/build-it-yourself/
[signoff]: https://git-scm.com/docs/git-commit#Documentation/git-commit.txt--s
