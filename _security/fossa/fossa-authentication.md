---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Fossa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fossa secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fossa
provider_slug: fossa
scheme_count: 1
schemes:
- description: Every call to the FOSSA API authenticates with an API token passed as a Bearer token in the Authorization header, over HTTPS only.
  format: 'Authorization: Bearer [example key]'
  header: Authorization
  in: header
  name: apiToken
  scheme: bearer
  sources:
  - https://docs.fossa.com/docs/api/authentication
  type: http
slug: fossa-authentication
source_filename: fossa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.fossa.com/docs/api/authentication\ndocs: https://docs.fossa.com/docs/api/authentication\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  transport: https-only\nschemes:\n- name: apiToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Authorization: Bearer [example key]'\n  sources: [https://docs.fossa.com/docs/api/authentication]\n  description: >-\n    Every call to the FOSSA API authenticates with an API token passed as a\n    Bearer token in the Authorization header, over HTTPS only.\ncredential_forms:\n- name: personal-api-token\n  description: Individual user credential tied to that user's permissions.\n- name: service-account\n  description: Non-human credential for automation and integrations.\n- name: oidc\n  description: >-\n    Short-lived JWT exchanged from a CI/CD platform's OIDC identity for a FOSSA\n    token — no long-lived secret stored in the pipeline.\n\
  access_levels:\n- name: push-only\n  description: Can send/push analysis data to FOSSA but not read.\n- name: full\n  description: Read/write access equivalent to the account's permissions.\ntoken_management:\n- rotation_docs: https://docs.fossa.com/docs/api/examples/rotating-access-tokens\nnotes:\n- The FOSSA CLI reads its token from the FOSSA_API_KEY environment variable.\n- No OAuth2 authorization/token flow or scopes are published for the REST API; access is API-token based, so no scopes/ artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fossa/refs/heads/main/authentication/fossa-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Software Supply Chain
- Open Source
- License Compliance
- Vulnerability Management
- SBOM
- Software Composition Analysis
- DevSecOps
---
