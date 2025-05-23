# Windows TEST DISA STIG

## Configure a Windows 10 Enterprise system to be [DISA STIG](https://public.cyber.mil/stigs/downloads/) compliant.

### Based on [ Windows DISA STIG Version 3, Rel 3 released on April 2nd, 2025 ](https://dl.dod.cyber.mil/wp-content/uploads/stigs/zip/U_MS_Windows_10_V3R4_STIG.zip)

---

## Public Repository 📣

![Org Stars](https://img.shields.io/github/stars/ansible-lockdown?label=Org%20Stars&style=social)
![Stars](https://img.shields.io/github/stars/ansible-lockdown/Windows-Test?label=Repo%20Stars&style=social)
![Forks](https://img.shields.io/github/forks/ansible-lockdown/Windows-Test?style=social)
![Followers](https://img.shields.io/github/followers/ansible-lockdown?style=social)
[![Twitter URL](https://img.shields.io/twitter/url/https/twitter.com/AnsibleLockdown.svg?style=social&label=Follow%20%40AnsibleLockdown)](https://twitter.com/AnsibleLockdown)
![Discord Badge](https://img.shields.io/discord/925818806838919229?logo=discord)
<!-- ![Ansible Galaxy Quality](https://img.shields.io/ansible/quality/61846?label=Quality&&logo=ansible) -->

![License](https://img.shields.io/github/license/ansible-lockdown/Windows-Test?label=License)

## Lint & Pre-Commit Tools 🔧

[![Pre-Commit.ci](https://img.shields.io/endpoint?url=https://ansible-lockdown.github.io/github_windows_IaC/badges/Windows-Test/pre-commit-ci.json)](https://results.pre-commit.ci/latest/github/ansible-lockdown/Windows-Test/devel)
![YamlLint](https://img.shields.io/badge/yamllint-Present-brightgreen?style=flat&logo=yaml&logoColor=white)
![Ansible-Lint](https://img.shields.io/badge/ansible--lint-Present-brightgreen?style=flat&logo=ansible&logoColor=white)

## Community Release Information 📂

![Release Branch](https://img.shields.io/badge/Release%20Branch-Main-brightgreen)
![Release Tag](https://img.shields.io/github/v/tag/ansible-lockdown/Windows-Test?label=Release%20Tag&&color=success)
![Main Release Date](https://img.shields.io/github/release-date/ansible-lockdown/Windows-Test?label=Release%20Date)
![Benchmark Version Main](https://img.shields.io/endpoint?url=https://ansible-lockdown.github.io/github_windows_IaC/badges/Windows-Test/benchmark-version-main.json)
![Benchmark Version Devel](https://img.shields.io/endpoint?url=https://ansible-lockdown.github.io/github_windows_IaC/badges/Windows-Test/benchmark-version-devel.json)

[![Main Pipeline Status](https://github.com/ansible-lockdown/Windows-Test/actions/workflows/main_pipeline_validation.yml/badge.svg?)](https://github.com/ansible-lockdown/Windows-Test/actions/workflows/main_pipeline_validation.yml)

[![Devel Pipeline Status](https://github.com/ansible-lockdown/Windows-Test/actions/workflows/devel_pipeline_validation.yml/badge.svg?)](https://github.com/ansible-lockdown/Windows-Test/actions/workflows/devel_pipeline_validation.yml)

![Devel Commits](https://img.shields.io/github/commit-activity/m/ansible-lockdown/Windows-Test/devel?color=dark%20green&label=Devel%20Branch%20Commits)
![Open Issues](https://img.shields.io/github/issues-raw/ansible-lockdown/Windows-Test?label=Open%20Issues)
![Closed Issues](https://img.shields.io/github/issues-closed-raw/ansible-lockdown/Windows-Test?label=Closed%20Issues&&color=success)
![Pull Requests](https://img.shields.io/github/issues-pr/ansible-lockdown/Windows-Test?label=Pull%20Requests)

---

## Subscriber Release Information 🔐

![Private Release Branch](https://img.shields.io/endpoint?url=https://ansible-lockdown.github.io/github_windows_IaC/badges/Private-Windows-Test/release-branch.json)
![Private Benchmark Version](https://img.shields.io/endpoint?url=https://ansible-lockdown.github.io/github_windows_IaC/badges/Private-Windows-Test/benchmark-version.json)

[![Private Remediate Pipeline](https://img.shields.io/endpoint?url=https://ansible-lockdown.github.io/github_windows_IaC/badges/Private-Windows-Test/remediate.json)](https://github.com/ansible-lockdown/Private-Windows-Test/actions/workflows/main_pipeline_validation.yml)

![Private Pull Requests](https://img.shields.io/endpoint?url=https://ansible-lockdown.github.io/github_windows_IaC/badges/Private-Windows-Test/prs.json)
![Private Closed Issues](https://img.shields.io/endpoint?url=https://ansible-lockdown.github.io/github_windows_IaC/badges/Private-Windows-Test/issues-closed.json)

---


## Looking For Support? 🤝

[Lockdown Enterprise](https://www.lockdownenterprise.com#GH_AL_WINDOWS_10_stig)

[Ansible Support](https://www.mindpointgroup.com/cybersecurity-products/ansible-counselor#GH_AL_WINDOWS_10_stig)

### Community 💬

Join us on our [Discord Server](https://www.lockdownenterprise.com/discord) to ask questions, discuss features, or just chat with other Ansible-Lockdown users.

---

## 🚨 Caution(s) 🚨

This role **will make changes to the system** which may have unintended consequences. This is not an auditing tool but rather a remediation tool to be used after an audit has been conducted.

Check Mode is not supported! 🚫 The role will complete in check mode without errors, but it is not supported and should be used with caution.

This role was developed against a clean install of the Windows 10. If you are implementing to an existing system please review this role for any site specific changes that are needed.

To use release version please point to main branch and relevant release for the stig benchmark you wish to work with.

---

## Matching A Security Level For STIG 🔐

It is possible to to only run controls that are based on a particular for security level for STIG.
This is managed using tags:

- CAT1
- CAT2
- CAT3

The controls found in defaults/main also need to reflect those control numbers due to aligning every control to the audit component.

## Coming From A Previous Release ⏪

STIG releases always contain changes, it is highly recommended to review the new references and available variables. This has changed significantly since the initial release of ansible-lockdown.
This is now compatible with python3 if it is found to be the default interpreter. This does come with pre-requisites which it configures the system accordingly.

Further details can be seen in the [Changelog](./ChangeLog.md)

## Auditing (new) 🔍

Currently this release does not have a auditing tool that is up to date.

## Documentation 📖

- [Read The Docs](https://ansible-lockdown.readthedocs.io/en/latest/)
- [Getting Started](https://www.lockdownenterprise.com/docs/getting-started-with-lockdown#GH_AL_WINDOWS_10_stig)
- [Customizing Roles](https://www.lockdownenterprise.com/docs/customizing-lockdown-enterprise#GH_AL_WINDOWS_10_stig)
- [Per-Host Configuration](https://www.lockdownenterprise.com/docs/per-host-lockdown-enterprise-configuration#GH_AL_WINDOWS_10_stig)
- [Getting the Most Out of the Role](https://www.lockdownenterprise.com/docs/get-the-most-out-of-lockdown-enterprise#GH_AL_WINDOWS_10_stig)

## Requirements ✅

**General:**

- Basic knowledge of Ansible, below are some links to the Ansible documentation to help get started if you are unfamiliar with Ansible

  - [Main Ansible documentation page](https://docs.ansible.com)
  - [Ansible Getting Started](https://docs.ansible.com/ansible/latest/user_guide/intro_getting_started.html)
  - [Tower User Guide](https://docs.ansible.com/ansible-tower/latest/html/userguide/index.html)
  - [Ansible Community Info](https://docs.ansible.com/ansible/latest/community/index.html)
- Functioning Ansible and/or Tower Installed, configured, and running. This includes all of the base Ansible/Tower configurations, needed packages installed, and infrastructure setup.
- Please read through the tasks in this role to gain an understanding of what each control is doing. Some of the tasks are disruptive and can have unintended consiquences in a live production system. Also familiarize yourself with the variables in the defaults/main.yml file.

**Technical Dependencies:** ⚙️

- Windows 10 Enterprise 22H2 - Other versions are not supported
- Running Ansible/Tower setup (this role is tested against Ansible version 2.10.1 and newer)
- Python3 Ansible run environment
- passlib (or python2-passlib, if using python2)
- python-lxml
- python-xmltodict
- python-jmespath
- pywinrm

Package 'python-xmltodict' is required if you enable the OpenSCAP tool installation and run a report. Packages python(2)-passlib and python-jmespath are required for tasks with custom filters or modules. These are all required on the controller host that executes Ansible.

## Role Variables 📋

This role is designed so that the end user should not have to edit the tasks themselves. All customizing should be done via the defaults/main.yml file or with extra vars within the project, job, workflow, etc.

## Tags 🏷️

There are many tags available for added control precision. Each control has its own set of tags noting what level, what OS element it relates to, whether it's a patch or audit, and the rule number. Additionally, NIST references follow a specific conversion format for consistency and clarity.

### Conversion Format for NIST References:

  1. Standard Prefix:

    - All references are prefixed with "NIST SP".

  2. Standard Types:

    - "800-53" references are formatted as NIST800-53.
    - "800-53A" references are formatted as NIST800-53A.
    - "800-53r4" references are formatted as NIST800-53R4 (with 'R' capitalized).

  3. Details:

    - Section and subsection numbers use periods (.) for numeric separators.
    - Parenthetical elements are separated by underscores (_), e.g., IA-5(1)(d) becomes IA-5_1_d.
    - Subsection letters (e.g., "b") are appended with an underscore.

### Example of Tag Usage:
Below is an example of the tag section from a control within this role. Using this example, if you set your run to skip all controls with the tag CCI-000018, this task will be skipped. Conversely, you can choose to run only controls tagged with CCI-000018.

```sh
tags:
      - WN10-AU-000040
      - CAT2
      - CCI-000018
      - CCI-000172
      - CCI-001403
      - CCI-001404
      - CCI-001405
      - CCI-002130
      - CCI-002234
      - SRG-OS-000004-GPOS-00004
      - SV-220752r958368_rule
      - V-220752
      - NIST800-53_AC-2_4
      - NIST800-53_AU-12_c
      - NIST800-53A_AC-2_4.1_i&ii
      - NIST800-53A_AC-12.1_iv
      - NIST800-53R4_AC-2_4
      - NIST800-53R4_AU-12_c
```
### Conversion Examples in Use:
  - NIST SP 800-53 :: AC-2 (4) → NIST800-53_AC-2_4
  - NIST SP 800-53A :: AC-2 (4).1 (i&ii) → NIST800-53A_AC-2_4.1_i&ii
  - NIST SP 800-53 Revision 4 :: AC-2 (4) → NIST800-53_AC-2_4
  - NIST SP 800-53 :: AU-12 c → NIST800-53_AU-12_c
  - NIST SP 800-53A :: AU-12.1 (iv) → NIST800-53A_AC-12.1_iv
  - NIST SP 800-53 Revision 4 :: AU-12 c →  NIST800-53R4_AU-12_c

By maintaining this consistent tagging structure, it becomes easier to filter and manage tasks based on specific controls and compliance requirements.

## Community Contribution 🧑‍🤝‍🧑

We encourage you (the community) to contribute to this role. Please read the rules below.

- Your work is done in your own individual branch. Make sure to Signed-off and GPG sign all commits you intend to merge.
- All community Pull Requests are pulled into the devel branch.
- Pull Requests into devel will confirm your commits have a GPG signature, Signed-off, and a functional test before being approved.
- Once your changes are merged and a more detailed review is complete, an authorized member will merge your changes into the main branch for a new release.

## Pipeline Testing 🔄

uses:

- ansible-core 2.16.x
- ansible collections - pulls in the latest version based on requirements file
- runs the audit using the devel branch
- This is an automated test that occurs on pull requests into devel
- self-hosted runners using OpenTofu

## Local Testing 💻

  - Ansible
    - ansible-core 2.18.2 - python 3.13

## Credits and Thanks 🙏

Massive thanks to the fantastic community and all its members.

This includes a huge thanks and credit to the original authors and maintainers.

