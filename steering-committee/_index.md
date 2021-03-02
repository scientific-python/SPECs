---
title: "SPEC Steering Committee"
date: 2021-01-06
draft: true
author:
  - "Jarrod Millman <millman@berkeley.edu>"
  - "Stéfan van der Walt <stefanv@berkeley.edu>"
---

# Description

The SPEC process is managed by the Steering Committee.
The Steering Committee represents the interests of the ecosystem and the community.
The Steering Committee also represent the interests of the
[Core Projects]({{< relref "/specs/core-projects" >}})
and is composed partially of individuals who are active Core Project contributors.
In particular, the Steering Committee members

- monitor the
  [SPECs discussion forum](https://discuss.scientific-python.org/c/specs/6),
- determine which proposed SPECs are accepted as described in the SPEC
  [Purpose and Process]({{< relref "/specs/purpose-and-process" >}}),
- approve changes to the SPEC process including to the
  [SPEC Purpose and Process]({{< relref "/specs/purpose-and-process" >}}),
  [SPEC Steering Committee]({{< relref "/specs/steering-committee" >}}), and
  [SPEC Core Projects]({{< relref "/specs/core-projects" >}}), as well as
- serve as a communication channel to and from projects they contribute to as
  well as the larger ecosystem.

The Steering Committee decides which SPECs are _accepted_, but not
which SPECs are _adopted_—that choice resides with individual
projects.
Similarly, the Steering Committee does not decide which SPECs are _endorsed_—that
choice resides with individual core projects.

## Steering Committee

{{< page_gallery pages="." >}}

# Implementation

Public communication takes place in the
[`specs` GitHub repository](https://github.com/scientific-python/specs/)
and the [SPECs discussion forum](https://discuss.scientific-python.org/c/specs/6).
Private communication within the Steering Committee takes place on
[Steering Committee private mailing list](https://groups.io/g/spec-steering-committee/).
Steering Committee members are expected to be aware of conversations on this list to lend validity
to consensus-seeking and voting.

## How are SPECs accepted?

To accept a SPEC (i.e., assigning it a SPEC number, marking its discussion
`Accepted`, and merging the pull request) requires two members of the Steering
Committee to approve and no members objecting.
Since the role of the Steering Committee is mainly to ensure that SPEC proposals are
appropriate,[^accept] objections should be rare.

## How is the SPEC process changed?

The Steering Committee makes decisions about changing the SPEC process documents
([SPEC Purpose and Process]({{< relref "/specs/purpose-and-process" >}}),
[SPEC Steering Committee]({{< relref "/specs/steering-committee" >}}), and
[SPEC Core Projects]({{< relref "/specs/core-projects" >}}))
through group consensus and, in the very rare instance
where no consensus can be reached, by two-thirds majority vote of those
available to cast a vote within ten days.

## Who should be a member?

Members of the Steering Committee should be active in the scientific Python ecosystem and
should have a demonstrated interest in the Core Projects and the SPEC process.
Examples of demonstrated interest include submitting SPECs, engaging in SPEC
discussions, reviewing SPEC pull requests, or advocating for wider SPEC participation.
Members of the steering committee do not have to belong to a core project.

## How many members should there be?

This is up to the Steering Committee.
However, if the Steering Committee is unable to quickly handle new SPEC proposals and new ideas arising
in the discussions aren't addressed in a timely manner, the Steering Committee should try to
recruit new members.

## How do you add a member?

If the Steering Committee decides to admit a new member and that person agrees,
then they should be added to the
(1) the Steering Committee member listing above,
(2) the [Steering Committee Team](https://github.com/orgs/scientific-python/teams/spec-steering-committee/members),
(3) the [Steering Committee Discourse Group](https://discuss.scientific-python.org/g/SSC), and
(4) the [Steering Committee private mailing list](https://groups.io/g/spec-steering-committee/members).

## How do you remove a member?

If a member wishes to resign or if the Steering Committee decides to remove a member,
then they should
(1) be moved to the list of Emeritus Steering Committee members (below the list of active members),
(2) be removed from the
[Steering Committee Team](https://github.com/orgs/scientific-python/teams/spec-steering-committee/members),
(3) be removed from the
[Steering Committee Discourse Group](https://discuss.scientific-python.org/g/SSC), and
(4) be removed from the [Steering Committee private mailing list](https://groups.io/g/spec-steering-committee/members).

# Notes

[^accept]:
    Proposed SPECs are accepted once (a) the draft is written to clearly explain the area of
    common concern and a general approach to a shared solution and (b) there
    are contributors (from at least two Core Projects) interested in working on the new SPEC
    and in championing it to their projects as well as the larger community.
