## Definition of Done

**Note:** If any of the following are not done at the time of PR review, the PR should only be accepted if it links to appropriate issues on the backlog for that repo that covers the incomplete criteria.

- Repo name:
  - [ ] Prefixed with `ansible-role-`
  - [ ] Noun based (e.g. `nginx`) not verb based (e.g. `build-nginx`)
  - [ ] Aligns with convention for SAP-related roles (e.g. `ansible-role-sap-hana-backup`)
- Repo meta data/config:
  - [ ] Tagged with `ansible-role`
  - [ ] Description consistent for service catalogue (e.g. `Centiq’s Ansible role for managing ...`)
  - [ ] Centiq Staff have write access
  - [ ] Centiq Service Accounts have read access
- [ ] Standard ansible role `.gitignore`
- [README](README.md) contains:
  - [ ] Level 1 heading title of the form: `Ansible Role: ...`
  - [ ] Build status badge for the `master` branch just beneath the title
  - [ ] High-level description of the role (no more than a paragraph)
  - [ ] All main subsections:
    - [ ] `Requirements`
    - [ ] `Role Variables` with defaults
    - [ ] `Role Testing` with detail of how to test
    - [ ] `Example Playbook` with a working example (or a link to one)
    - [ ] `License` set to `Centiq Commercial in Confidence Source Code License` that links to the correct license file
    - [ ] `Author Information` set and linked to the `Centiq Engineering Team`
- [Travis Build](.travis.yml):
  - [ ] Exists and is passing in Travis
  - [ ] Running either:
    - `molecule test`
    - `molecule lint` (with a backlog issue for moving to `molecule test`)
  - [ ] Running against:
    - CentOS 7
  - [ ] Slack status notifications using an encrypted access token
- Release:
  - [ ] v0.0.1 has been released (or will be immediately after the PR merge)
  - [ ] Deploy key setup
