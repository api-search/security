---
api_key_in:
- environment
- parameter
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tensor9 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tensor9 secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Tensor9
provider_slug: tensor9
scheme_count: 2
schemes:
- description: API key supplied to the tensor9 CLI via the T9_API_KEY environment variable. Required by most commands.
  in: environment
  name: T9_API_KEY
  parameter: T9_API_KEY
  sources:
  - https://docs.tensor9.com/cli/reference.md
  type: apiKey
- description: API key passed directly to a tensor9 command via the -apiKey flag as an alternative to the T9_API_KEY environment variable.
  in: parameter
  name: apiKey-flag
  parameter: -apiKey
  sources:
  - https://docs.tensor9.com/cli/reference.md
  type: apiKey
slug: tensor9-authentication
source_filename: tensor9-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tensor9.com/cli/reference.md\ndocs: https://docs.tensor9.com/cli/reference.md\nsummary:\n  types: [apiKey]\n  api_key_in: [environment, parameter]\n  oauth2_flows: []\n  notes: >-\n    Tensor9's programmatic surface is its CLI/control plane, authenticated with a\n    vendor API key. Tensor9 does not publish a public REST/OpenAPI API, so there\n    are no OpenAPI-declared securitySchemes to derive from; this profile is taken\n    from the documented CLI authentication model.\nschemes:\n  - name: T9_API_KEY\n    type: apiKey\n    in: environment\n    parameter: T9_API_KEY\n    description: >-\n      API key supplied to the tensor9 CLI via the T9_API_KEY environment\n      variable. Required by most commands.\n    sources: [https://docs.tensor9.com/cli/reference.md]\n  - name: apiKey-flag\n    type: apiKey\n    in: parameter\n    parameter: -apiKey\n    description: >-\n      API key passed directly to a tensor9 command\
  \ via the -apiKey flag as an\n      alternative to the T9_API_KEY environment variable.\n    sources: [https://docs.tensor9.com/cli/reference.md]\nrelated:\n  - customer-side security model: https://docs.tensor9.com/customer/security/security-model.md\n  - credentials and secrets: https://docs.tensor9.com/customer/security/credentials-and-secrets.md\n  - signing keys: https://docs.tensor9.com/customer/security/signing-keys.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tensor9/refs/heads/main/authentication/tensor9-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Deployment
- BYOC
- Cloud Portability
- Infrastructure as Code
- Kubernetes
- On-Premises
- Security
- DevOps
- CLI
---
