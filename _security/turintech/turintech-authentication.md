---
api_key_in:
- config
- env
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Turintech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Turintech secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Turintech
provider_slug: turintech
scheme_count: 2
schemes:
- in: config-or-env
  name: ARTEMIS_API_KEY
  parameter: ARTEMIS_API_KEY
  scope: Artemis platform access
  sources:
  - https://docs.artemis.turintech.ai/features/artemis-cli
  type: apiKey
- in: managed-credential
  name: git-provider-token
  parameter: token
  providers:
  - github
  - gitlab
  - bitbucket
  - azure-devops
  scope: Git repository access (per provider PAT)
  sources:
  - https://docs.artemis.turintech.ai/features/artemis-cli
  type: apiKey
slug: turintech-authentication
source_filename: turintech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.artemis.turintech.ai/features/artemis-cli\ndocs: https://docs.artemis.turintech.ai\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - config\n  - env\n  oauth2_flows: []\n  note: >-\n    The Artemis platform is accessed through the Artemis CLI/platform using a\n    single API key (ARTEMIS_API_KEY), configured via `artemis config set\n    ARTEMIS_API_KEY <key>` or the ARTEMIS_API_KEY environment variable. Separate\n    Git provider tokens (GitHub/GitLab/Bitbucket/Azure DevOps personal access\n    tokens) are registered with `artemis key add` for repository access. No\n    public OpenAPI or OAuth flow is documented; auth is derived from published\n    CLI documentation, not a machine-readable spec.\nschemes:\n- name: ARTEMIS_API_KEY\n  type: apiKey\n  in: config-or-env\n  parameter: ARTEMIS_API_KEY\n  scope: Artemis platform access\n  sources:\n  - https://docs.artemis.turintech.ai/features/artemis-cli\n- name:\
  \ git-provider-token\n  type: apiKey\n  in: managed-credential\n  parameter: token\n  scope: Git repository access (per provider PAT)\n  providers:\n  - github\n  - gitlab\n  - bitbucket\n  - azure-devops\n  sources:\n  - https://docs.artemis.turintech.ai/features/artemis-cli\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/turintech/refs/heads/main/authentication/turintech-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Code Optimization
- Developer Tools
- DevOps
- Large Language Models
- Agentic AI
- CLI
---
