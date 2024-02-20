# Sigstore Best Practices Badge Application - Passing

_Note: this is evidence of adherence to Best Practices across all of Sigstore’s projects._

Basics

### Identification

#### What is the human-readable name of the project? 

sigstore

#### What is a brief description of the project? 

Sigstore is an open source project for improving software supply chain security. The Sigstore framework and tooling empowers software developers and consumers to securely sign and verify software artifacts such as release files, container images, binaries, software bills of materials (SBOMs), SLSA provenance, in-toto attestations and more. Signatures are generated with ephemeral signing keys so there’s no need to manage keys. Signing events are recorded in a tamper-resistant public log so software developers can audit signing events.

#### What is the URL for the project (as a whole)? 

[https://www.sigstore.dev](https://www.sigstore.dev)

#### What is the URL for the version control repository (it may be the same as the project URL)?

[https://github.com/sigstore/](https://github.com/sigstore/)

#### What programming language(s) are used to implement the project? 

Go, Java, Python, Rust

#### What is the Common Platform Enumeration (CPE) name for the project (if it has one)? 

[cpe:2.3:a:sigstore](https://nvd.nist.gov/products/cpe/search/results?namingFormat=2.3\&orderBy=2.3\&keyword=cpe%3A2.3%3Aa%3Asigstore\&status=FINAL)

### Basic project website content

#### The project website MUST succinctly describe what the software does (what problem does it solve?).

[https://www.sigstore.dev](https://www.sigstore.dev)

#### The project website MUST provide information on how to: obtain, provide feedback (as bug reports or enhancements), and contribute to the software.

Sigstore projects are hosted on GitHub, and by default use issues (as encouraged by documentation such as [https://guides.github.com/activities/contributing-to-open-source/](https://guides.github.com/activities/contributing-to-open-source/)).

#### The information on how to contribute MUST explain the contribution process (e.g., are pull requests used?)

Sigstore projects are hosted on GitHub, and by default use issues and pull requests, as encouraged by documentation such as [https://guides.github.com/activities/contributing-to-open-source/](https://guides.github.com/activities/contributing-to-open-source/).

#### The information on how to contribute SHOULD include the requirements for acceptable contributions (e.g., a reference to any required coding standard).

[https://github.com/sigstore/community/blob/main/CONTRIBUTORS.md](https://github.com/sigstore/community/blob/main/CONTRIBUTORS.md)

### FLOSS license

#### What license(s) is the project released under? 

Apache 2.0

#### The software produced by the project MUST be released as FLOSS.

As required by the OpenSSF Charter, all software artifacts produced by Sigstore are Apache 2 licensed.

#### It is SUGGESTED that any required license(s) for the software produced by the project be approved by the Open Source Initiative (OSI).

Apache 2 is an OSI-approved license: [https://opensource.org/license/apache-2-0/](https://opensource.org/license/apache-2-0/)

#### The project MUST post the license(s) of its results in a standard location in their source repository. 

Each Sigstore repository has a LICENSE file in the root of the repository.

### Documentation

#### The project MUST provide basic documentation for the software produced by the project.

[https://docs.sigstore.dev/](https://docs.sigstore.dev/)

#### The project MUST provide reference documentation that describes the external interface (both input and output) of the software produced by the project. 

[https://github.com/sigstore/protobuf-specs](https://github.com/sigstore/protobuf-specs)

### Other

#### The project sites (website, repository, and download URLs) MUST support HTTPS using TLS.

All of Sigstore’s public sites and services all support HTTPS via TLS.

#### The project MUST have one or more mechanisms for discussion (including proposed changes and issues) that are searchable, allow messages and topics to be addressed by URL, enable new people to participate in some of the discussions, and do not require client-side installation of proprietary software.

GitHub supports discussions on issues and pull requests.

#### The project SHOULD provide documentation in English and be able to accept bug reports and comments about code in English.

Documentation in English is available at [https://docs.sigstore.dev](https://docs.sigstore.dev)

#### The project MUST be maintained.

Sigstore projects are actively maintained; evidence is available on GitHub.

## Change Control

### Public version-controlled source repository

#### The project MUST have a version-controlled source repository that is publicly readable and has a URL. 

Repository on GitHub, which provides public git repositories with URLs.

#### The project's source repository MUST track what changes were made, who made the changes, and when the changes were made.

Repository on GitHub, which uses git. git can track the changes, who made them, and when they were made.

#### To enable collaborative review, the project's source repository MUST include interim versions for review between releases; it MUST NOT include only final releases.

GitHub pull requests support this feature.

#### It is SUGGESTED that common distributed version control software be used (e.g., git) for the project's source repository.

Sigstore hosts its code on GitHub, which uses git.

### Unique version numbering

#### The project results MUST have a unique version identifier for each release intended to be used by users. 

Releases published from [https://github.com/sigstore/](https://github.com/sigstore/) repos use GitHub Releases, which have unique version numbers.

#### It is SUGGESTED that the Semantic Versioning (SemVer) or Calendar Versioning (CalVer) version numbering format be used for releases. It is SUGGESTED that those who use CalVer include a micro level value.

We adhere to semantic versioning for the clients and services, and have a [declared policy](https://github.com/sigstore/cosign/blob/main/VERSIONING.md) documenting this.It is SUGGESTED that projects identify each release within their version control system. For example, it is SUGGESTED that those using git identify each release using git tags.Sigstore uses Git Tags for each release.

#### The project MUST provide, in each release, release notes that are a human-readable summary of major changes in that release to help users determine if they should upgrade and what the upgrade impact will be. The release notes MUST NOT be the raw output of a version control log (e.g., the "git log" command results are not release notes). Projects whose results are not intended for reuse in multiple locations (such as the software for a single website or service) AND employ continuous delivery MAY select "N/A".

Sigstore projects publish changelogs as a part of each release (example at [https://github.com/sigstore/sigstore/releases/tag/v1.1.0](https://github.com/sigstore/sigstore/releases/tag/v1.1.0))The release notes MUST identify every publicly known run-time vulnerability fixed in this release that already had a CVE assignment or similar when the release was created. This criterion may be marked as not applicable (N/A) if users typically cannot practically update the software themselves (e.g., as is often true for kernel updates). This criterion applies only to the project results, not to its dependencies. If there are no release notes or there have been no publicly known vulnerabilities, choose N/A. Sigstore projects publish changelogs with CVEs fixed as a part of each release (example at [https://github.com/sigstore/cosign/releases/tag/v2.2.1](https://github.com/sigstore/cosign/releases/tag/v2.2.1))

## Reporting

### Bug-reporting process

#### The project MUST provide a process for users to submit bug reports (e.g., using an issue tracker or a mailing list).  

Evidence of use of GitHub Issues can be seen across various GitHub repositories under the [Sigstore organization](http://github.com/sigstore).

#### The project SHOULD use an issue tracker for tracking individual issues.

Evidence of use of GitHub Issues can be seen across various GitHub repositories under the [Sigstore organization](http://github.com/sigstore).

#### The project MUST acknowledge a majority of bug reports submitted in the last 2-12 months (inclusive); the response need not include a fix.

Evidence of this can be seen across various GitHub repositories under the [Sigstore organization](http://github.com/sigstore).

#### The project SHOULD respond to a majority (>50%) of enhancement requests in the last 2-12 months (inclusive). 

Evidence of this can be seen across various GitHub repositories under the [Sigstore organization](http://github.com/sigstore).

#### The project MUST have a publicly available archive for reports and responses for later searching.

Evidence of use of GitHub Issues can be seen across various GitHub repositories under the [Sigstore organization](http://github.com/sigstore).

### Vulnerability report process

#### The project MUST publish the process for reporting vulnerabilities on the project site.

[https://github.com/sigstore/.github/blob/main/SECURITY.md](https://github.com/sigstore/.github/blob/main/SECURITY.md)

#### If private vulnerability reports are supported, the project MUST include how to send the information in a way that is kept private.

Users have an option to send the vulnerability privately and it is documented here: [https://github.com/sigstore/.github/blob/main/SECURITY.md](https://github.com/sigstore/.github/blob/main/SECURITY.md)

#### The project's initial response time for any vulnerability report received in the last 6 months MUST be less than or equal to 14 days. 

We have adhered to this response SLO for all issues reported to the Security Response Committee.

## Quality

### Working build system

#### If the software produced by the project requires building for use, the project MUST provide a working build system that can automatically rebuild the software from source code. 

Each project within Sigstore can be rebuilt using idiomatic FLOSS build tools for the respective language, and are regularly built in GitHub Actions.

#### It is SUGGESTED that common tools be used for building the software.

Each project within Sigstore can be rebuilt using idiomatic FLOSS build tools for the respective language, and are regularly built in GitHub Actions.

#### The project SHOULD be buildable using only FLOSS tools.

Each project within Sigstore can be rebuilt using idiomatic FLOSS build tools for the respective language, and are regularly built in GitHub Actions.

### Automated test suite

#### The project MUST use at least one automated test suite that is publicly released as FLOSS (this test suite may be maintained as a separate FLOSS project). The project MUST clearly show or document how to run the test suite(s) (e.g., via a continuous integration (CI) script or via documentation in files such as BUILD.md, README.md, or CONTRIBUTING.md). 

Each project within Sigstore is tested using idiomatic FLOSS testing tools for the respective language, and are regularly tested in GitHub Actions for each pull request.A test suite SHOULD be invocable in a standard way for that language. 

#### It is SUGGESTED that the test suite cover most (or ideally all) the code branches, input fields, and functionality.

Several key projects within Sigstore use Codecov to measure code coverage.

#### It is SUGGESTED that the project implement continuous integration (where new or changed code is frequently integrated into a central code repository and automated tests are run on the result). 

Each project within Sigstore is tested using idiomatic FLOSS testing tools for the respective language, and are regularly tested in GitHub Actions for each pull request.

### New functionality testing

#### The project MUST have a general policy (formal or not) that as major new functionality is added to the software produced by the project, tests of that functionality should be added to an automated test suite. 

This is a general principle within sigstore, with evidence present across our repositories.

#### The project MUST have evidence that the test\_policy for adding tests has been adhered to in the most recent major changes to the software produced by the project.

This is a general principle within sigstore, with evidence present across our repositories.

#### It is SUGGESTED that this policy on adding tests (see test\_policy) be documented in the instructions for change proposals. 

This has not been done yet, but is a good idea.

### Warning flags

#### The project MUST enable one or more compiler warning flags, a "safe" language mode, or use a separate "linter" tool to look for code quality errors or common simple mistakes, if there is at least one FLOSS tool that can implement this criterion in the selected language.

We use golangci-lint in our Go projects, and CodeQL as well.

#### The project MUST address warnings.

Linting issues are in required tests which must pass to merge a PR.

#### It is SUGGESTED that projects be maximally strict with warnings in the software produced by the project, where practical. 

Our linting configs are stored in source control and can be audited for strictness. 

## Security

### Secure development knowledge

#### The project MUST have at least one primary developer who knows how to design secure software. (See ‘details’ for the exact requirements.)

Several of our maintainers work in security engineering departments (e.g. Google’s Open Source Security Team).

#### At least one of the project's primary developers MUST know of common kinds of errors that lead to vulnerabilities in this kind of software, as well as at least one method to counter or mitigate each of them. 

Several of our maintainers work in security engineering departments (e.g. Google’s Open Source Security Team).

### Use basic good cryptographic practices

Note that some software does not need to use cryptographic mechanisms. If your project produces software that (1) includes, activates, or enables encryption functionality, and (2) might be released from the United States (US) to outside the US or to a non-US-citizen, you may be legally required to take a few extra steps. Typically this just involves sending an email. For more information, see the encryption section of Understanding Open Source Technology & US Export Controls.

#### The software produced by the project MUST use, by default, only cryptographic protocols and algorithms that are publicly published and reviewed by experts (if cryptographic protocols and algorithms are used). 

All of Sigstore’s use of cryptographic protocols come from either a language’s standard library, or from well-vetted FLOSS libraries.

#### If the software produced by the project is an application or library, and its primary purpose is not to implement cryptography, then it SHOULD only call on software specifically designed to implement cryptographic functions; it SHOULD NOT re-implement its own.

Sigstore does not implement new cryptographic functions, but re-uses well-known FLOSS libraries to provide that functionality.

#### All functionality in the software produced by the project that depends on cryptography MUST be implementable using FLOSS.

Sigstore does not implement new cryptographic functions, but re-uses well-known FLOSS libraries to provide that functionality.

#### The security mechanisms within the software produced by the project MUST use default keylengths that at least meet the NIST minimum requirements through the year 2030 (as stated in 2012). It MUST be possible to configure the software so that smaller keylengths are completely disabled. 

Sigstore does not implement new cryptographic functions, but re-uses well-known FLOSS libraries with strong defaults (key length, PRNGs).

#### The default security mechanisms within the software produced by the project MUST NOT depend on broken cryptographic algorithms (e.g., MD4, MD5, single DES, RC4, Dual\_EC\_DRBG), or use cipher modes that are inappropriate to the context, unless they are necessary to implement an interoperable protocol (where the protocol implemented is the most recent version of that standard broadly supported by the network ecosystem, that ecosystem requires the use of such an algorithm or mode, and that ecosystem does not offer any more secure alternative). The documentation MUST describe any relevant security risks and any known mitigations if these broken algorithms or modes are necessary for an interoperable protocol. 

Sigstore re-uses well-known FLOSS cryptography libraries with strong defaults, and as such does not proliferate use of any broken algorithms.

#### The default security mechanisms within the software produced by the project SHOULD NOT depend on cryptographic algorithms or modes with known serious weaknesses (e.g., the SHA-1 cryptographic hash algorithm or the CBC mode in SSH). 

Sigstore re-uses well-known FLOSS cryptography libraries with strong defaults, and as such does not proliferate use of any broken algorithms.

#### The security mechanisms within the software produced by the project SHOULD implement perfect forward secrecy for key agreement protocols so a session key derived from a set of long-term keys cannot be compromised if one of the long-term keys is compromised in the future. 

Not applicable

#### If the software produced by the project causes the storing of passwords for authentication of external users, the passwords MUST be stored as iterated hashes with a per-user salt by using a key stretching (iterated) algorithm (e.g., Argon2id, Bcrypt, Scrypt, or PBKDF2). See also OWASP Password Storage Cheat Sheet). 

Not applicable

#### The security mechanisms within the software produced by the project MUST generate all cryptographic keys and nonces using a cryptographically secure random number generator, and MUST NOT do so using generators that are cryptographically insecure. 

Sigstore re-uses well-known FLOSS cryptography libraries with strong defaults, and as such does not proliferate use of any broken algorithms.

### Secured delivery against man-in-the-middle (MITM) attacks

#### The project MUST use a delivery mechanism that counters MITM attacks. Using https or ssh+scp is acceptable. 

HTTPS is used for all communications between Sigstore clients and services.

#### A cryptographic hash (e.g., a sha1sum) MUST NOT be retrieved over http and used without checking for a cryptographic signature. 

Sigstore’s purpose is to have developers sign & verify software they use ;)

### Publicly known vulnerabilities fixed

#### There MUST be no unpatched vulnerabilities of medium or higher severity that have been publicly known for more than 60 days.

There are no unpatched vulnerabilities.

#### Projects SHOULD fix all critical vulnerabilities rapidly after they are reported. 

All critical vulnerabilities have been immediately patched and fixed in a new release with a corresponding CVE.

### Other security issues

#### The public repositories MUST NOT leak a valid private credential (e.g., a working password or private key) that is intended to limit public access. 

We rely on secret scanning in GitHub to ensure we do not leak credentials.

## Analysis

### Static code analysis

#### At least one static code analysis tool (beyond compiler warnings and "safe" language modes) MUST be applied to any proposed major production release of the software before its release, if there is at least one FLOSS tool that implements this criterion in the selected language. 

We leverage CodeQL: https\://github.com/sigstore/sigstore/blob/main/.github/workflows/codeql.yml

#### It is SUGGESTED that at least one of the static analysis tools used for the static\_analysis criterion include rules or approaches to look for common vulnerabilities in the analyzed language or environment. 

We leverage CodeQL: https\://github.com/sigstore/sigstore/blob/main/.github/workflows/codeql.yml

#### All medium and higher severity exploitable vulnerabilities discovered with static code analysis MUST be fixed in a timely way after they are confirmed. 

All vulnerabilities discovered are handled according to the Sigstore [SECURITY.MD](http://security.md) process

#### It is SUGGESTED that static source code analysis occur on every commit or at least daily. 

We have CodeQL running on each PR or nightly on each repo.

### Dynamic code analysis

#### It is SUGGESTED that at least one dynamic analysis tool be applied to any proposed major production release of the software before its release. 

We regularly fuzz our key projects; e.g. [https://github.com/sigstore/sigstore/blob/main/.github/workflows/fuzzing.yml](https://github.com/sigstore/sigstore/blob/main/.github/workflows/fuzzing.yml)

#### It is SUGGESTED that if the software produced by the project includes software written using a memory-unsafe language (e.g., C or C++), then at least one dynamic tool (e.g., a fuzzer or web application scanner) be routinely used in combination with a mechanism to detect memory safety problems such as buffer overwrites. If the project does not produce software written in a memory-unsafe language, choose "not applicable" (N/A). 

We regularly fuzz our key projects; e.g. [https://github.com/sigstore/sigstore/blob/main/.github/workflows/fuzzing.yml](https://github.com/sigstore/sigstore/blob/main/.github/workflows/fuzzing.yml)

#### It is SUGGESTED that the project use a configuration for at least some dynamic analysis (such as testing or fuzzing) which enables many assertions. In many cases these assertions should not be enabled in production builds.

We regularly fuzz our key projects; e.g. [https://github.com/sigstore/sigstore/blob/main/.github/workflows/fuzzing.yml](https://github.com/sigstore/sigstore/blob/main/.github/workflows/fuzzing.yml)

#### All medium and higher severity exploitable vulnerabilities discovered with dynamic code analysis MUST be fixed in a timely way after they are confirmed.

Issues found via fuzzers are triaged and handled in the same way as vulnerability disclosures.

# Sigstore Best Practices Badge Application - Silver

_Note: this is evidence of adherence to Best Practices across all of Sigstore’s projects._

## Basics

### Prerequisites

#### The project MUST achieve a passing level badge.

See above; we believe we meet all passing level criteria

### Basic project website content

#### The information on how to contribute MUST include the requirements for acceptable contributions (e.g., a reference to any required coding standard).

[https://github.com/sigstore/community/blob/main/CONTRIBUTORS.md](https://github.com/sigstore/community/blob/main/CONTRIBUTORS.md)

### Project oversight

#### The project SHOULD have a legal mechanism where all developers of non-trivial amounts of project software assert that they are legally authorized to make these contributions. The most common and easily-implemented approach for doing this is by using a Developer Certificate of Origin (DCO), where users add "signed-off-by" in their commits and the project links to the DCO website. However, this MAY be implemented as a Contributor License Agreement (CLA), or other legal mechanism. 

DCO is enforced on all Sigstore projects per the OpenSSF requirement.

#### The project MUST clearly define and document its project governance model (the way it makes decisions, including key roles). 

Sigstore’s charter & TSC is documented at [https://github.com/sigstore/TSC/blob/main/docs/CHARTER.MD](https://github.com/sigstore/TSC/blob/main/docs/CHARTER.MD) 

#### The project MUST adopt a code of conduct and post it in a standard location. 

Sigstore’s Code of Conduct can be found at [https://github.com/sigstore/.github/blob/main/CODE\_OF\_CONDUCT.md](https://github.com/sigstore/.github/blob/main/CODE_OF_CONDUCT.md) 

#### The project MUST clearly define and publicly document the key roles in the project and their responsibilities, including any tasks those roles must perform. It MUST be clear who has which role(s), though this might not be documented in the same way. 

Roles in Sigstore are defined in [https://github.com/sigstore/community/blob/main/MEMBERSHIP.md](https://github.com/sigstore/community/blob/main/MEMBERSHIP.md) with who has which roles as defined in the Pulumi configuration visible at [https://github.com/sigstore/community/tree/main/github-sync/github-data/sigstore](https://github.com/sigstore/community/tree/main/github-sync/github-data/sigstore) 

#### The project MUST be able to continue with minimal interruption if any one person dies, is incapacitated, or is otherwise unable or unwilling to continue support of the project. In particular, the project MUST be able to create and close issues, accept proposed changes, and release versions of software, within a week of confirmation of the loss of support from any one individual. This MAY be done by ensuring someone else has any necessary keys, passwords, and legal rights to continue the project. Individuals who run a FLOSS project MAY do this by providing keys in a lockbox and a will providing any needed legal rights (e.g., for DNS names).

All credentials required to merge PRs, operate the Sigstore service, are controlled by the TSC, a 5 person group. Each project has at least two maintainers.

#### The project SHOULD have a "bus factor" of 2 or more. 

All credentials required to merge PRs, operate the Sigstore service, are controlled by the TSC, a 5 person group. Each project has at least two maintainers.

### Documentation

#### The project MUST have a documented roadmap that describes what the project intends to do and not do for at least the next year. 

The Sigstore Roadmap can be seen at [https://github.com/sigstore/community/blob/main/ROADMAP.md](https://github.com/sigstore/community/blob/main/ROADMAP.md) 

#### The project MUST include documentation of the architecture (aka high-level design) of the software produced by the project. If the project does not produce software, select "not applicable" (N/A). 

We are in the process of converting these into Markdown on our docs site, but can be seen in Google Doc form at [https://docs.google.com/document/d/1-OccxmZwkZZItrfOnO3RP8gku6nRbtJpth1mSW3U1Cc/edit#heading=h.ksk0rwk2ti2e](https://docs.google.com/document/d/1-OccxmZwkZZItrfOnO3RP8gku6nRbtJpth1mSW3U1Cc/edit#heading=h.ksk0rwk2ti2e) 

#### The project MUST document what the user can and cannot expect in terms of security from the software produced by the project (its "security requirements"). 

Our documentation contains both a [security model](https://docs.sigstore.dev/about/security/) and a [threat model.](https://docs.sigstore.dev/about/threat-model/)

#### The project MUST provide a "quick start" guide for new users to help them quickly do something with the software.  

[https://docs.sigstore.dev/signing/quickstart/](https://docs.sigstore.dev/signing/quickstart/) 

#### The project MUST make an effort to keep the documentation consistent with the current version of the project results (including software produced by the project). Any known documentation defects making it inconsistent MUST be fixed. If the documentation is generally current, but erroneously includes some older information that is no longer true, just treat that as a defect, then track and fix as usual. 

Our docs are reasonably current, and we accept PRs to update and fix errors if they are found.

#### The project repository front page and/or website MUST identify and hyperlink to any achievements, including this best practices badge, within 48 hours of public recognition that the achievement has been attained. 

Need to complete this

### Accessibility and internationalization

#### The project (both project sites and project results) SHOULD follow accessibility best practices so that persons with disabilities can still participate in the project and use the project results where it is reasonable to do so.

#### The software produced by the project SHOULD be internationalized to enable easy localization for the target audience's culture, region, or language. If internationalization (i18n) does not apply (e.g., the software doesn't generate text intended for end-users and doesn't sort human-readable text), select "not applicable" (N/A).

### Other

#### If the project sites (website, repository, and download URLs) store passwords for authentication of external users, the passwords MUST be stored as iterated hashes with a per-user salt by using a key stretching (iterated) algorithm (e.g., Argon2id, Bcrypt, Scrypt, or PBKDF2). If the project sites do not store passwords for this purpose, select "not applicable" (N/A)

N/A, as we do not store user passwords.

## Change Control

### Previous versions

#### The project MUST maintain the most often used older versions of the product or provide an upgrade path to newer versions. If the upgrade path is difficult, the project MUST document how to perform the upgrade (e.g., the interfaces that have changed and detailed suggested steps to help upgrade). 

All previous releases are available to download from GitHub.

## Reporting

### Bug-reporting process

#### The project MUST use an issue tracker for tracking individual issues. 

We use GitHub Issues for all issue tracking.

### Vulnerability report process

#### The project MUST give credit to the reporter(s) of all vulnerability reports resolved in the last 12 months, except for the reporter(s) who request anonymity. If there have been no vulnerabilities resolved in the last 12 months, select "not applicable" (N/A).

We have given credit to the reporters of all CVEs that the project has ever received.

#### The project MUST have a documented process for responding to vulnerability reports.

[https://github.com/sigstore/.github/blob/main/SECURITY.md](https://github.com/sigstore/.github/blob/main/SECURITY.md) 

## Quality

### Coding standards

#### The project MUST identify the specific coding style guides for the primary languages it uses, and require that contributions generally comply with it.  

We enforce coding standards via golangci-lint.

#### The project MUST automatically enforce its selected coding style(s) if there is at least one FLOSS tool that can do so in the selected language(s). 

We enforce coding standards via golangci-lint.

### Working build system

#### Build systems for native binaries MUST honor the relevant compiler and linker (environment) variables passed in to them (e.g., CC, CFLAGS, CXX, CXXFLAGS, and LDFLAGS) and pass them to compiler and linker invocations. A build system MAY extend them with additional flags; it MUST NOT simply replace provided values with its own. If no native binaries are being generated, select "not applicable" (N/A). 

Our makefiles provide for LDFLAG overrides if desired.

#### The build and installation system SHOULD preserve debugging information if they are requested in the relevant flags (e.g., "install -s" is not used). If there is no build or installation system (e.g., typical JavaScript libraries), select "not applicable" (N/A). 

We do not strip our binaries.

#### The build system for the software produced by the project MUST NOT recursively build subdirectories if there are cross-dependencies in the subdirectories. If there is no build or installation system (e.g., typical JavaScript libraries), select "not applicable" (N/A). 

N/A

#### The project MUST be able to repeat the process of generating information from source files and get exactly the same bit-for-bit result. If no building occurs (e.g., scripting languages where the source code is used directly instead of being compiled), select "not applicable" (N/A). 

N/A

### Installation system

#### The project MUST provide a way to easily install and uninstall the software produced by the project using a commonly-used convention. 

We support installing via GitHub CLI, Homebrew, and package cosign and other CLIs via popular distributions.

#### The installation system for end-users MUST honor standard conventions for selecting the location where built artifacts are written to at installation time. For example, if it installs files on a POSIX system it MUST honor the DESTDIR environment variable. If there is no installation system or no standard convention, select "not applicable" (N/A). 

N/A

#### The project MUST provide a way for potential developers to quickly install all the project results and support environment necessary to make changes, including the tests and test environment. This MUST be performed with a commonly-used convention. 

We follow standard conventions for each programming language we use for this.

### Externally-maintained components

#### The project MUST list external dependencies in a computer-processable way.  

We list external dependencies in a language-appropriate lock file.

#### Projects MUST monitor or periodically check their external dependencies (including convenience copies) to detect known vulnerabilities, and fix exploitable vulnerabilities or verify them as unexploitable. 

We use actions/dependency-review-action to monitor dependencies for vulnerabilities in each project.

#### The project MUST either:make it easy to identify and update reused externally-maintained components; or use the standard components provided by the system or programming language. Then, if a vulnerability is found in a reused component, it will be easy to update that component. 

We use language-normative approaches for this.

#### The project SHOULD avoid using deprecated or obsolete functions and APIs where FLOSS alternatives are available in the set of technology it uses (its "technology stack") and to a supermajority of the users the project supports (so that users have ready access to the alternative). 

N/A

### Automated test suite

#### An automated test suite MUST be applied on each check-in to a shared repository for at least one branch. This test suite MUST produce a report on test success or failure. 

We run regression tests as part of GitHub Actions runs.

#### The project MUST add regression tests to an automated test suite for at least 50% of the bugs fixed within the last six months. 

We run regression tests as part of GitHub Actions runs, and require new tests for fixed bugs.

#### The project MUST have FLOSS automated test suite(s) that provide at least 80% statement coverage if there is at least one FLOSS tool that can measure this criterion in the selected language. 

We use CodeCov & go coverage tools to measure coverage.

### New functionality testing

#### The project MUST have a formal written policy that as major new functionality is added, tests for the new functionality MUST be added to an automated test suite. 

Sigstore does not have a change management process persay, but typically expects test coverage as a culture norm.

#### The project MUST include, in its documented instructions for change proposals, the policy that tests are to be added for major new functionality. 

Sigstore does not have a change management process persay, but typically expects test coverage as a culture norm.

### Warning flags

#### Projects MUST be maximally strict with warnings in the software produced by the project, where practical. 

We use the default, strict settings in linters to look for warnings.

## Security

### Secure development knowledge

#### The project MUST implement secure design principles (from "know\_secure\_design"), where applicable. If the project is not producing software, select "not applicable" (N/A). 

Sigstore’s contributor base tends to be security-aware engineers who follow secure design principles.

### Use basic good cryptographic practices

#### Note that some software does not need to use cryptographic mechanisms. If your project produces software that (1) includes, activates, or enables encryption functionality, and (2) might be released from the United States (US) to outside the US or to a non-US-citizen, you may be legally required to take a few extra steps. Typically this just involves sending an email. For more information, see the encryption section of Understanding Open Source Technology & US Export Controls.

N/A

#### The default security mechanisms within the software produced by the project MUST NOT depend on cryptographic algorithms or modes with known serious weaknesses (e.g., the SHA-1 cryptographic hash algorithm or the CBC mode in SSH.

We do not use weak algorithms or ciphers.

#### The project SHOULD support multiple cryptographic algorithms, so users can quickly switch if one is broken. Common symmetric key algorithms include AES, Twofish, and Serpent. Common cryptographic hash algorithm alternatives include SHA-2 (including SHA-224, SHA-256, SHA-384 AND SHA-512) and SHA-3. 

We do support cryptographic agility, as evidenced by recent work to support PQ algorithms.

#### The project MUST support storing authentication credentials (such as passwords and dynamic tokens) and private cryptographic keys in files that are separate from other information (such as configuration files, databases, and logs), and permit users to update and replace them without code recompilation. If the project never processes authentication credentials and private cryptographic keys, select "not applicable" (N/A). 

N/A

#### The software produced by the project SHOULD support secure protocols for all of its network communications, such as SSHv2 or later, TLS1.2 or later (HTTPS), IPsec, SFTP, and SNMPv3. Insecure protocols such as FTP, HTTP, telnet, SSLv3 or earlier, and SSHv1 SHOULD be disabled by default, and only enabled if the user specifically configures it. If the software produced by the project does not support network communications, select "not applicable" (N/A). 

We mandate TLS1.2+ in all communications within our infrastructure.

#### The software produced by the project SHOULD, if it supports or uses TLS, support at least TLS version 1.2. Note that the predecessor of TLS was called SSL. If the software does not use TLS, select "not applicable" (N/A). 

We mandate TLS1.2+ in all communications within our infrastructure.

#### The software produced by the project MUST, if it supports TLS, perform TLS certificate verification by default when using TLS, including on subresources. If the software does not use TLS, select "not applicable" (N/A).

We mandate TLS1.2+ in all communications within our infrastructure with mandatory validation.

#### The software produced by the project MUST, if it supports TLS, perform certificate verification before sending HTTP headers with private information (such as secure cookies). If the software does not use TLS, select "not applicable" (N/A).

We mandate TLS1.2+ in all communications within our infrastructure with mandatory validation.

### Secure release

#### The project MUST cryptographically sign releases of the project results intended for widespread use, and there MUST be a documented process explaining to users how they can obtain the public signing keys and verify the signature(s). The private key for these signature(s) MUST NOT be on site(s) used to directly distribute the software to the public. If releases are not intended for widespread use, select "not applicable" (N/A). 

We sign all our releases with Sigstore, of course :)

#### It is SUGGESTED that in the version control system, each important version tag (a tag that is part of a major release, minor release, or fixes publicly noted vulnerabilities) be cryptographically signed and verifiable as described in signed\_releases. 

Go releases have this property inherently.

### Other security issues

#### The project results MUST check all inputs from potentially untrusted sources to ensure they are valid (an \*allowlist\*), and reject invalid inputs, if there are any restrictions on the data at all. 

We do input validation checking as part of our API handlers.

#### Hardening mechanisms SHOULD be used in the software produced by the project so that software defects are less likely to result in security vulnerabilities.

#### The project MUST provide an assurance case that justifies why its security requirements are met. The assurance case MUST include: a description of the threat model, clear identification of trust boundaries, an argument that secure design principles have been applied, and an argument that common implementation security weaknesses have been countered. 

[https://docs.sigstore.dev/about/threat-model](https://docs.sigstore.dev/about/threat-model)

## Analysis

### Static code analysis

#### The project MUST use at least one static analysis tool with rules or approaches to look for common vulnerabilities in the analyzed language or environment, if there is at least one FLOSS tool that can implement this criterion in the selected language. 

We leverage CodeQL in Sigstore; example available @ https\://github.com/sigstore/sigstore/blob/main/.github/workflows/codeql.yml

### Dynamic code analysis

#### If the software produced by the project includes software written using a memory-unsafe language (e.g., C or C++), then at least one dynamic tool (e.g., a fuzzer or web application scanner) MUST be routinely used in combination with a mechanism to detect memory safety problems such as buffer overwrites. If the project does not produce software written in a memory-unsafe language, choose "not applicable" (N/A).

We regularly fuzz our key projects; e.g. [https://github.com/sigstore/sigstore/blob/main/.github/workflows/fuzzing.yml](https://github.com/sigstore/sigstore/blob/main/.github/workflows/fuzzing.yml)

# Sigstore Best Practices Badge Application - Gold

_Note: this is evidence of adherence to Best Practices across all of Sigstore’s projects._

## Basics

### Project oversight

#### The project MUST have a "bus factor" of 2 or more.  

All credentials required to merge PRs, operate the Sigstore service, are controlled by the TSC, a 5 person group. Each project has at least two maintainers.

#### The project MUST have at least two unassociated significant contributors.  

All credentials required to merge PRs, operate the Sigstore service, are controlled by the TSC, a 5 person group representing unique organizations. Each project has at least two maintainers.

### Other

#### The project MUST include a copyright statement in each source file, identifying the copyright holder.

All source files include a copyright statement at the top.

#### The project MUST include a license statement in each source file. This MAY be done by including the following inside a comment near the beginning of each file: SPDX-License-Identifier: 

Each project contains a LICENSE file that denotes the license for all files in the repository.

## Change Control

### Public version-controlled source repository

#### The project's source repository MUST use a common distributed version control software (e.g., git or mercurial). 

Repository on GitHub, which uses git. git is distributed.

#### The project MUST clearly identify small tasks that can be performed by new or casual contributors.  

We do occasionally use the first\_good\_issue tag, though we could get better about this.

#### The project MUST require two-factor authentication (2FA) for developers for changing a central repository or accessing sensitive data (such as private vulnerability reports). This 2FA mechanism MAY use mechanisms without cryptographic mechanisms such as SMS, though that is not recommended. 

We mandate 2FA for our GitHub organization, as well as hardware-backed MFA for our infrastructure.

## Quality

### Coding standards

#### The project MUST document its code review requirements, including how code review is conducted, what must be checked, and what is required to be acceptable.  

We do not document this yet.

#### The project MUST have at least 50% of all proposed modifications reviewed before release by a person other than the author, to determine if it is a worthwhile modification and free of known issues which would argue against its inclusion 

We use two party commit review rules across all projects.

### Working build system

#### The project MUST have a reproducible build. If no building occurs (e.g., scripting languages where the source code is used directly instead of being compiled), select "not applicable" (N/A).  

For all languages where this is practically possible, we build in a reproducible manner.

### Automated test suite

#### A test suite MUST be invocable in a standard way for that language.  

All test suites are invoked in an idiomatic way.

#### The project MUST implement continuous integration, where new or changed code is frequently integrated into a central code repository and automated tests are run on the result. 

We use GitHub Actions across all of Sigstore.

#### The project MUST have FLOSS automated test suite(s) that provide at least 90% statement coverage if there is at least one FLOSS tool that can measure this criterion in the selected language. 

We’re currently at around 60%+ coverage on most projects.

#### The project MUST have FLOSS automated test suite(s) that provide at least 80% branch coverage if there is at least one FLOSS tool that can measure this criterion in the selected language.

We’re currently at around 60%+ coverage on most projects.

## Security

### Use basic good cryptographic practices

#### Note that some software does not need to use cryptographic mechanisms. If your project produces software that (1) includes, activates, or enables encryption functionality, and (2) might be released from the United States (US) to outside the US or to a non-US-citizen, you may be legally required to take a few extra steps. Typically this just involves sending an email. For more information, see the encryption section of Understanding Open Source Technology & US Export Controls.

Ack

#### The software produced by the project MUST support secure protocols for all of its network communications, such as SSHv2 or later, TLS1.2 or later (HTTPS), IPsec, SFTP, and SNMPv3. Insecure protocols such as FTP, HTTP, telnet, SSLv3 or earlier, and SSHv1 MUST be disabled by default, and only enabled if the user specifically configures it. If the software produced by the project does not support network communications, select "not applicable" (N/A). 

Sigstore mandates a minimum of TLSv1.2 in all communications.

#### The software produced by the project MUST, if it supports or uses TLS, support at least TLS version 1.2. Note that the predecessor of TLS was called SSL. If the software does not use TLS, select "not applicable" (N/A). 

Sigstore mandates a minimum of TLSv1.2 in all communications.

### Secured delivery against man-in-the-middle (MITM) attacks

#### The project website, repository (if accessible via the web), and download site (if separate) MUST include key hardening headers with nonpermissive values.  

#### // X-Content-Type-Options was not set to "nosniff".

GitHub controls these headers, so Sigstore can not manage them directly.

### Other security issues

#### The project MUST have performed a security review within the last 5 years. This review MUST consider the security requirements and security boundary. 

OSTIF has reviewed several projects within Sigstore (Rekor, Fulcio, Cosign, sigstore-go)

#### Hardening mechanisms MUST be used in the software produced by the project so that software defects are less likely to result in security vulnerabilities. 

## Analysis

### Dynamic code analysis

#### The project MUST apply at least one dynamic analysis tool to any proposed major production release of the software produced by the project before its release. 

We regularly fuzz our key projects; e.g. [https://github.com/sigstore/sigstore/blob/main/.github/workflows/fuzzing.yml](https://github.com/sigstore/sigstore/blob/main/.github/workflows/fuzzing.yml)

#### The project SHOULD include many run-time assertions in the software it produces and check those assertions during dynamic analysis. 

We do not include assertions at this time.
