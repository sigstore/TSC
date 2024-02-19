*tl/dr: It is the shared view of the Sigstore Technical Steering Committee that Sigstore meets the requirements of a **Graduated** project within the OpenSSF:*

# Issue 162 response:

In response to the specific questions raised in [OpenSSF TAC Issue 162](https://github.com/ossf/tac/issues/162):

 <https://github.com/sigstore/community/blob/main/README.md> is a file that contains:

  - Link to our Slack instance, mailing list, and community calendar

  - [www.sigstore.dev](http://www.sigstore.dev) contains an overview of the project, [docs.sigstore.dev](https://docs.sigstore.dev/) contains technical documentation for the project

  - Bob Callaway is a member of both the OpenSSF TAC and Sigstore TSC (and acting as TAC sponsor of this request)

  - We have two formalized sub-groups:

    - [SIG-Clients](https://github.com/sigstore/sig-clients)

    - [SIG-Public-Good-Operations](https://github.com/sigstore/sig-public-good-operations)

- A clearly discoverable list of active members and their various levels can be found codified in YAML in users.yaml and teams.yaml at <https://github.com/sigstore/community/tree/main/github-sync/github-data/sigstore> 

  - Membership criteria and voting procedures are documented at <https://github.com/sigstore/community/blob/main/MEMBERSHIP.md> 

- An [up-to-date charter](https://github.com/sigstore/TSC/blob/main/docs/CHARTER.MD) is located under the [sigstore/tsc repo](https://github.com/sigstore/tsc)

- Our GitHub-organization-wide [security.MD](https://github.com/sigstore/.github/blob/main/SECURITY.md) file covers our disclosure reporting process

  - 4-member security response team responsible for triaging reported issues

# Per the [criteria specified on the OpenSSF TAC repo](https://github.com/ossf/tac/blob/main/process/project-lifecycle.md#graduated) for a graduated project:

## Responsibilities:

- Provided updates to OpenSSF TAC on _8/9/22, 10/4/22, 8/8/23, 11/14/23_

  - [OpenSSF TAC Meeting Notes (2022-04-05..2023-12-12)](https://docs.google.com/document/d/1706vJpuyq4NpHpVYsOTeU90j5RpoJREX7MRlhAo-CW4/edit#heading=h.d8z1b876r79s)

- We maintain a diversified contributor base with an active flow of contributions

  - [58 repositories](https://github.com/orgs/sigstore/repositories?q=\&type=all\&language=\&sort=stargazers) spanning polyglot client SDKs, servers (transparency logs, certificate authorities, policy controllers), supporting automation (e.g. Helm charts and Terraform templates)

  - Examples of contributor/maintainer diversity:

    - Cosign: [Contributor data](https://github.com/sigstore/cosign/graphs/contributors)

      - Maintainers from: Chainguard, Google, Trendyol 

    - Sigstore-python: [Contributor data](https://github.com/sigstore/sigstore-python/graphs/contributors) 

      - Maintainers from: Google, Trail of Bits, Stacklok

    - Sigstore-rs: [Contributor data](https://github.com/sigstore/sigstore-rs/graphs/contributors)

      - Maintainers from: Alibaba, Google, Red Hat, Stacklok, SUSE, Stacklok 

- We follow security best practices (Scorecard, AllStar, Dependabot & CodeQL support, build pipelines automated through CI/CD, branch protection). For the services we operate, infrastructure is hardened, access for oncall engineers is on-demand with review, and we use the latest cloud technologies to manage infrastructure (GKE, Helm, Terraform)

  - Writeup available here: [Sigstore Best Practices Badge Application](best_practices_badge.md)

  - _FYI: The current Best Practices badge is done on a per-repo basis; I’ve compiled the responses in the above doc to demonstrate our application against the criteria_

- We maintain a point of contact for vulnerability reports as documented in [security.MD](https://github.com/sigstore/.github/blob/main/SECURITY.md) and follow coordinated vulnerability disclosure practices.

- We implement and practice mature development & release processes. We leverage automated CI/CD for testing and releases, with releases built on Google Cloud Build and GitHub Actions. Releases are signed with Sigstore. We adhere to semantic versioning for the clients and services, and have a [declared policy](https://github.com/sigstore/cosign/blob/main/VERSIONING.md) documenting this. Clients must meet a minimum bar for a GA/1.0 release ([example with Rust](https://github.com/sigstore/sigstore-rs/issues/274)).

## Support:

- We receive guidance from the OpenSSF TAC while providing updates to the TAC.

- Sigstore is represented in OpenSSF conferences through the supply chain security track.

- Each Sigstore repository includes a [code of conduct](https://github.com/sigstore/sigstore/blob/main/CODE_OF_CONDUCT.md).

- Follows [vulnerability disclosure practices](https://github.com/sigstore/.github/blob/main/SECURITY.md) as documented in the Vulnerability Disclosure WG.

- Project updates are regularly posted to [blog.sigstore.dev](https://blog.sigstore.dev/) and to the OpenSSF blog. The Linux Foundation offers a [training course](https://training.linuxfoundation.org/training/securing-your-software-supply-chain-with-sigstore-lfs182x/) for Sigstore.

## Requirements:

- Sigstore has maintainers across many different companies and academic institutions (Examples include Purdue, NYU, Google, Chainguard, GitHub, RedHat, Stacklok, Trail of Bits)

- Sigstore represents a novel approach to digital signing, removing the need for signing key management and providing an auditable record of signatures. Sigstore provides a trust foundation for other OpenSSF projects (SLSA, Scorecard, OpenVex).

- Sigstore has become the de-facto approach to code signing for open source projects. As seen on [Sigstore's Landscape](https://landscape.openssf.org/sigstore), major adopters include Kubernetes, Helm, Python and Kyverno. In 2024 and beyond, package repositories are the focus for adoption, to improve supply chain security for package ecosystems. npm leverages Sigstore to sign SLSA provenance statements, a feature which went into general availability last year. Homebrew, PyPI and Maven Central Sigstore integration is actively underway for each ecosystem.

- Clients and services receive regular updates and release frequently (approximately a monthly cadence, or as needed for bug fixes)

- [Project governance is documented](https://github.com/sigstore/community/blob/main/MEMBERSHIP.md) and seen through updates to the community repository to update maintainers.

  - TSC Meeting minutes are available at [Sigstore TSC Agenda and Minutes](https://docs.google.com/document/d/1rN_tn2Jf1hd_e6XDLlKg0vmQog3LIxEHfulG50WzgKQ/edit#heading=h.x9j826571elg)

- OSTIF completed [a security audit](https://openssf.org/blog/2022/07/18/results-of-sigstore-and-slf4j-security-audits/) for Sigstore, with all findings addressed.
