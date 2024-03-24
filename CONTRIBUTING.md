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

[![Static Badge](https://img.shields.io/badge/git-email-f34c27?style=for-the-badge&logo=git&logoColor=f34c27)](#i-dont-want-to-use-github)
![Static Badge](https://img.shields.io/badge/Contributions-welcome!-3DA639?style=for-the-badge&logo=open-source-initiative&logoColor=3DA639)
[![Contributor Covenant](https://img.shields.io/badge/Code-of%20conduct-4baaaa.svg?style=for-the-badge)][coc] 

<!-- insert
{{< rawhtml >}}
</div>
{{< /rawhtml >}}
end_insert -->

Thanks for considering contributing!

To keep things simple, [my projects][oss] all follow these common guidelines.

## TL;DR

If you just want to fix a typo or another very small thing, just create a PR.

## Documentation

As the author of a tool or library, we are blind to many of the problems that users may encounter. As an external person, you have the power to spot this! Feel free to open an issue or to send a PR with proposed changes to the documentation.

## Code

### Pull Request

* It is advisable, **but not mandatory**, to create an issue to discuss the feature you want to add, so that you can make sure it has good chances to be merged. This also avoids having multiple persons working on the same thing.
  * Similarly, feel free to create a [draft PR][draft] with your changes before they are completed. This is useful to point to a particular part of the code during discussions.
* Try to create one pull request per high level feature or bug fix. Then if necessary [try to stage your changes][stage] by crafting multiple commits: if your commits follow a progression on your changes, it’ll be easier to review.

### I Don’t Want to Use GitHub

That’s fine, feel free to send your contributions by [email][] to the address listed in [Contact][contact].

### I Don’t Know What to Do

If you don’t know what to do, but still want to help, that’s great! Look for issues labeled [`good-first-issue`][gh-first] or [`help-wanted`][gh-help]. You can also [contact me][contact], and tell me about your interests and skills.

### Dependencies

As much as possible, I limit the number of dependencies used in my projects. Please avoid introducing new dependencies in your PRs if possible. The fewer dependencies, the better. The dependencies actually included should be relatively popular and from trusted authors, as I can’t audit any of them.

## Code of Conduct

To foster a welcoming environment, we also follow and enforce [a code of conduct][coc].

## See Also

The other [open-source documents][docs].

[coc]: https://cj.rs/docs/code-of-conduct/
[contact]: https://cj.rs/contact
[docs]: https://cj.rs/open-source/docs/
[draft]: https://github.blog/2019-02-14-introducing-draft-pull-requests/
[email]: https://git-send-email.io/
[gh-first]: https://github.com/search?q=user%3Acljoly+label%3A%22good+first+issue%22+state%3Aopen&type=Issues
[gh-help]: https://github.com/search?q=user%3Acljoly+label%3A%22help+wanted%22+state%3Aopen&type=Issues
[oss]: https://cj.rs/open-source
[stage]: https://github.blog/2022-06-30-write-better-commits-build-better-projects/#structure-the-narrative
