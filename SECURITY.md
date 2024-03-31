<!-- insert
---
title: "Security Policy"
summary: "Guidelines to report a security issue"
date: 2022-08-14T14:00:23+02:00
weight: 5000
draft: false
aliases:
  - "/docs/security"
---
end_insert -->

<!-- remove -->
# Security Policy
<!-- end_remove -->

<!-- insert
{{< rawhtml >}}
<div class="badges">
{{< /rawhtml >}}
end_insert -->

[![Contributions welcome!](https://img.shields.io/badge/Contributions_welcome!-3DA639?style=flat)][contrib]

<!-- insert
{{< rawhtml >}}
</div>
{{< /rawhtml >}}
end_insert -->

## Supported Versions

<!-- Use this section to tell people about which versions of your project are -->
<!-- currently being supported with security updates. -->

| Version                          | Supported          |
| -------                          |   :---------------:  |
| Latest tag                       | ✅                 |
| Latest commit on `master` or `main` | ✅                 |
| All other versions or commit     | ❌ |

## Reporting a Vulnerability

First, thanks for considering reporting!

You can [contact me][contact] and encrypt your message with one of the [keys][].
Please describe the issue as precisely as possible and don’t hesitate to propose a fix (for instance, with a [patch sent over email][sendmail]) if you have one.

<!-- Use this section to tell people how to report a vulnerability. -->

<!-- Tell them where to go, how often they can expect to get an update on a -->
<!-- reported vulnerability, what to expect if the vulnerability is accepted or -->
<!-- declined, etc. -->

## Signature

Commits and tags created after 2024-01-01 are signed with a key listed in [this file][allowed_signers].

The [blog post][post] gives more context and example of verification.

## Disclaimer

This policy is not a guarantee that my software will have the desired behavior or won’t cause harm. Please refer to the License of each software for the full disclaimer.

## See Also

The other [Open-Source documents][docs].

[allowed_signers]: https://cj.rs/.ssh/allowed_signers
[contact]: https://cj.rs/contact/
[contrib]: https://cj.rs/open-source/docs/contribute/
[docs]: https://cj.rs/open-source/docs/
[keys]: https://cj.rs/contact/#keys
[post]: https://cj.rs/blog/my-commits-and-tags-are-now-signed/
[sendmail]: https://git-send-email.io/
