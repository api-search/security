---
api_specs:
- filename: rest-api-description
  format: yaml
  label: GitHub API
  slug: github
  spec_type: OpenAPI
  url: https://github.com/github/rest-api-description
- filename: openapi.yaml
  format: yaml
  label: GitLab API
  slug: gitlab
  spec_type: OpenAPI
  url: https://docs.gitlab.com/ee/api/openapi/openapi.yaml
- filename: swagger
  format: yaml
  label: Gitea API
  slug: gitea
  spec_type: OpenAPI
  url: https://gitea.io/api/swagger
certifications: []
description: ''
kind: trust-center
layout: security
name: Git Trust Center
name_suffix: Trust Center
overview: Git maintains a public trust center covering its security and compliance posture.
provider_name: Git
provider_slug: git
slug: git-trust-center
source_filename: git-trust-center.yml
source_heading: Trust Center
source_url: ''
source_yaml: "generated: '2026-06-20'\nmethod: searched\nprobe: true\nsource: GitHub + GitLab public trust centers\ntrust_centers:\n  - provider: GitHub\n    url: https://ghec.github.trust.page/\n    certifications:\n      - ISO/IEC 27001:2013\n      - ISO/IEC 42001:2023\n      - CSA STAR Level 2\n      - SOC 1 Type 2\n      - SOC 2 Type 2\n      - SOC 3\n      - TISAX\n      - FedRAMP LI-SaaS\n    notes: >-\n      GitHub Enterprise Cloud with data residency is pursuing FedRAMP Moderate.\n      Copilot maintains a separate trust center at https://copilot.github.trust.page/.\n    evidence:\n      - {source: https://ghec.github.trust.page/, keywords: [soc 2, iso 27001, iso 42001, csa star, trust center]}\n  - provider: GitLab\n    url: https://trust.gitlab.com/\n    certifications:\n      - SOC 2 Type 2\n      - SOC 3\n      - ISO/IEC 27001:2022\n      - ISO/IEC 27017\n      - ISO/IEC 27018\n      - ISO/IEC 42001\n    notes: >-\n      Covers both GitLab.com and GitLab Dedicated. Trust center\
  \ powered by\n      SafeBase; certificates available in multiple languages.\n    evidence:\n      - {source: https://trust.gitlab.com/, keywords: [soc 2, iso 27001, iso 27017, iso 27018, iso 42001]}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/git/refs/heads/main/security/git-trust-center.yml
summary_line: trust center published
tags:
- Distributed
- Git
- Open Source
- Source Code Management
- Version Control
trust_url: ''
---
