---
title: "MetaSPEC 0 — Purpose and Process"
date: 2020-12-17
draft: false
author:
  - "Jarrod Millman <millman@berkeley.edu>"
  - "Stéfan van der Walt <stefanv@berkeley.edu>"
discussion: https://github.com/scientific-python/specs/discussions/9
---

# Description

Scientific Python Ecosystem Coordination documents or SPECs, for short, provide
operational guidelines for projects in the Scientific Python ecosystem.
Their goal is to coordinate the ecosystem and to provide a more unified
experience for users.

Projects in the ecosystem have an existing, diverse set of proposal processes
and development constraints.
SPECs, therefore, are not meant to be prescriptive: rather, they are a
mechanism to encourage shared practices and improve uniformity of experience.
SPECs may, for example, capture established practices so that new projects can
learn from them; or they may propose a new practice that the authors believe
will benefit the ecosystem as a whole.

Projects decide for themselves whether to adopt any given SPEC—often, this
would be through team consensus.
A SPEC may not be a good fit for every single project, and thus there is no
expectation that all SPECs must be adopted by all projects.
That said, SPECs only serve a meaningful purpose if they are adopted by several
projects—and their authority largely stems from the extent to which they are.

In practice, this means that SPECs will be tightly integrated with core
projects, but have to remain flexible enough for projects to implement them according
to their own constraints.

## Format

SPECs are UTF-8 encoded text files using
[Markdown](https://www.markdownguide.org/) format and stored in the [SPEC
repository](https://github.com/scientific-python/specs).
The SPEC documents are converted to HTML by code in the [scientific-python.org
repository](https://github.com/scientific-python/scientific-python.org/) using
[Hugo](https://gohugo.io/) and deployed to
[https://scientific-python.org/specs/](https://scientific-python.org/specs/).
Each SPEC has a corresponding
[discussion](https://github.com/scientific-python/specs/discussions/categories/specs)
with the same title, where anyone can comment, ask questions, or vote on
existing comments.
Often conversations about SPECs will occur on individual project's communication
channels (e.g., issues, pull requests, enhancement proposals, or commit messages).
It is the project's responsibility to link to these discussions on the official
[SPEC discussion](https://github.com/scientific-python/specs/discussions/categories/specs)
when appropriate.

# Implementation

Any community member can propose a new SPEC by making making a pull request to
the [SPEC repository](https://github.com/scientific-python/specs).
However, we highly recommended that the new proposal should first be discussed
in at least one important project in the ecosystem.
Often it is helpful also to have drafted a proof of concept implementation
for technical SPECs.

To get feedback from the larger community, we also recommend creating a new
[discussion](https://github.com/scientific-python/specs/discussions/new)—
selecting the
[Ideas](https://github.com/scientific-python/specs/discussions/categories/ideas)
category—as early in the process as possible.
The discussion will be linked to the new SPEC using the ``discussion``
field in the SPEC header.

Focus on a single key proposal or new idea for coordinating projects in
the scientific Python ecosystem.

Contributors must adhere to our [Code of Conduct]({{< relref
"/about/code_of_conduct.md" >}}).

## Create and submit a new SPEC

Creating a new SPEC requires (1) making a pull request with a new SPEC document (Markdown file) and (2) starting a related discussion.

To create a new SPEC document, use the ``quickstart.py`` script.
Located at the top-level of the [SPEC
repository](https://github.com/scientific-python/specs),
the script will ask you a few questions and then create a new file
appropriately named with a basic template for you to complete.

For example,

{{< highlight bash >}}
$ python quickstart.py
Enter your name: Jarrod Millman
Enter your email address: millman@berkeley.edu
Enter the SPEC number: 8
Enter the SPEC title: Minimum Supported Versions
Enter the discussion number: 13
{{< /highlight >}}

creates the file ``spec-0008.md`` containing:

{{< highlight markdown >}}
---
title: "SPEC 1 — Minimum Supported Versions"
date: 2021-01-10
draft: false
author:
  - "Jarrod Millman <millman@berkeley.edu>"
discussion: https://github.com/scientific-python/specs/discussions/13
adopted-by:
---

# Description

<!--
Briefly and clearly describe the proposal.
Explain the general need and the advantages of this specific proposal.
If relevant, include examples of how the new functionality would be
used, intended use-cases, and pseudo-code illustrating its use.
-->

# Implementation

<!--
Discuss how this would be implemented by projects.
-->

# Notes

<!--
Include a bulleted list of annotated links, comments, and other ancillary
information as needed.
-->

{{< /highlight >}}

When asked to enter the SPEC number, choose the next available number that
has not yet been used.
Before the SPEC is merged, the SSC may ask you to change the SPEC number so that
it doesn't conflict with another PR.
If so, just rename the file as appropriate and update the SPEC number in the
``title`` field of the SPEC header.

The script currently only supports adding one author.
If you need to add additional authors, just edit the text file.

For example, adding a second author the above template requires the following
change to the SPEC header:

{{< highlight markdown >}}
---
title: "SPEC 1 — Minimum Supported Versions"
date: 2021-01-10
draft: false
author:
  - "Jarrod Millman <millman@berkeley.edu>"
  - "Ross Barnowski <rossbar@berkeley.edu>"
discussion: https://github.com/scientific-python/specs/discussions/13
adopted-by:
---
{{< / highlight >}}

While it is recommended that you create a new discussion before creating the PR,
you can just make up a number when asked to enter the discussion number.
Before the PR is merged, you will be asked to verify that you've created a
new discussion and that the ``discussion`` field is correct.

Once the SPEC is in reasonable shape, file a pull request against the
[scientific-python/specs](https://github.com/scientific-python/specs)
repository.

## Review and Resolution

The SSC (see [MetaSPEC 1 — Governance and Decision Making]({{< relref
"/specs/meta-spec-0001.md" >}}) for details) will consider whether the new idea fits as a SPEC and
monitor subsequent discussion.
If there is sufficient interest, the SSC will convert the discussion to the
[SPEC](https://github.com/scientific-python/specs/discussions/categories/specs)
category and assign it a SPEC number.
When it is ready the SSC will merge the PR.
Additional PRs may be made to update or expand the SPEC.

## Enhancement Proposals and SPECs

For projects with an existing enhancement proposal process in place, we
recommend creating a new proposal to list the SPECs adopted along with links to
project discussions leading to adoption.

Once a project adopts a SPEC, they should add their project name to the
``adopted-by`` field in the SPEC header.

# Notes
