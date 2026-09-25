---
anonymous_access: false
api_key_in: []
api_specs:
- filename: booz-allen-hamilton-agile-api-openapi.yml
  format: yaml
  label: Booz Allen Hamilton Agile API
  slug: booz-allen-hamilton-agile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/booz-allen-hamilton/refs/heads/main/openapi/booz-allen-hamilton-agile-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Booz Allen Hamilton Authentication
name_suffix: Authentication
oauth_flows: []
overview: Booz Allen Hamilton declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Booz Allen Hamilton
provider_slug: booz-allen-hamilton
scheme_count: 0
schemes: []
slug: booz-allen-hamilton-authentication
source_filename: booz-allen-hamilton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: >-\n  https://github.com/boozallen/strands-base-agent/blob/develop/docs/foundry/configuration/environment-variables.md,\n  .../docs/foundry/guides/http-api.md, .../security/README.md and\n  https://raw.githubusercontent.com/boozallen/palm/main/openapi-specification.yaml — read 2026-09-14\nsummary: >-\n  There is no authentication to document for a Booz Allen API, because there is no Booz Allen API\n  to call. Both published contracts in the estate are for self-hosted software: the PALM\n  openapi-specification.yaml declares no components.securitySchemes at all, and the Agent Foundry\n  strands-base-agent baseline mounts its REST and A2A routes with no authn/authz layer, leaving\n  both to the adopter's deployment. This file records that measured absence — it is deliberately\n  NOT wired as an `Authentication` pointer in apis.yml, because crediting a documented auth model\n  here would assert a posture neither product has.\n\
  schemes: []\nderived_from_spec:\n  file: openapi/booz-allen-hamilton-palm-openapi.yaml\n  security_schemes: 0\n  note: PALM's published spec has no securitySchemes and no security requirement on its one operation.\nruntime_posture:\n  product: Agent Foundry — Strands Base Agent\n  built_in_authentication: none\n  responsibility: adopter (the fork/deployment)\n  transport_security:\n    tls: configurable in the runtime (TLS config module shipped in strands_base_agent)\n    cors:\n      env:\n        - {name: STRANDS_CORS_ORIGINS, default: localhost dev ports}\n        - {name: STRANDS_CORS_ALLOW_CREDENTIALS, default: 'false'}\n        - {name: STRANDS_CORS_ALLOW_METHODS, default: 'GET,POST,PUT,DELETE,OPTIONS,HEAD'}\n        - {name: STRANDS_CORS_ALLOW_HEADERS, default: 'Accept,Content-Type,Authorization,…'}\n  outbound_credentials:\n    - surface: MCP servers the agent calls\n      mechanism: per-server `headers` in config.yaml with ${VAR} substitution (e.g. Authorization Bearer)\n    \
  \  note: these authenticate the agent TO third-party services; they do not protect the agent's own endpoints\n    - surface: AWS Bedrock\n      mechanism: AWS_PROFILE / AWS_DEFAULT_REGION and the standard AWS credential chain\n  secrets_guidance: >-\n    \"Secrets (API keys, tokens, AWS credentials) should stay in .env files and never in config.yaml.\"\n  evidence:\n    stig_checklist: https://github.com/boozallen/strands-base-agent/blob/develop/security/stig_checklist.json\n    note: >-\n      The shipped DISA ASD STIG assessment covers the auth and authz domains explicitly; of 286\n      findings, 38 are marked `delivery` responsibility and 21 `shared`, which is where the adopter's\n      authentication work lands.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/booz-allen-hamilton/refs/heads/main/authentication/booz-allen-hamilton-authentication.yml
summary_line: 0 schemes
tags:
- Artificial Intelligence
- Consulting
- Cybersecurity
- Defense
- Federal Government
- Intelligence
- Management Consulting
- Technology
- Fortune 500
---
