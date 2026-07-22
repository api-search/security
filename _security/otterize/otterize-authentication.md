---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Otterize Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Otterize secures its APIs with oauth2 and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Otterize
provider_slug: otterize
scheme_count: 3
schemes:
- description: Interactive browser-based login to Otterize Cloud via `otterize login`; the CLI opens a browser to authenticate the user and stores the resulting credentials in ~/.otterize/config.
  flow: authorizationCode
  name: cloud-oauth-browser
  type: oauth2
- description: Non-interactive service authentication using a client id + client secret (`--client-id` / `--client-secret`), used by CI and by cluster-side integrations to obtain a token for the Otterize Cloud API.
  flow: clientCredentials
  name: cloud-client-credentials
  type: oauth2
- description: A pre-issued bearer token may be supplied directly via `--token` for the CLI / Cloud API calls.
  in: header
  name: cloud-token
  type: apiKey
slug: otterize-authentication
source_filename: otterize-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.otterize.com/reference/cli\nnote: >-\n  Otterize publishes no OpenAPI/GraphQL spec, so this profile is captured from the\n  documented Otterize Cloud API / CLI authentication surface rather than derived\n  from security schemes. The Otterize Cloud API is reached by the CLI and by\n  in-cluster operators.\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials]\nschemes:\n  - name: cloud-oauth-browser\n    type: oauth2\n    flow: authorizationCode\n    description: >-\n      Interactive browser-based login to Otterize Cloud via `otterize login`;\n      the CLI opens a browser to authenticate the user and stores the resulting\n      credentials in ~/.otterize/config.\n  - name: cloud-client-credentials\n    type: oauth2\n    flow: clientCredentials\n    description: >-\n      Non-interactive service authentication using a client id + client secret\n    \
  \  (`--client-id` / `--client-secret`), used by CI and by cluster-side\n      integrations to obtain a token for the Otterize Cloud API.\n  - name: cloud-token\n    type: apiKey\n    in: header\n    description: >-\n      A pre-issued bearer token may be supplied directly via `--token` for the\n      CLI / Cloud API calls.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/otterize/refs/heads/main/authentication/otterize-authentication.yml
summary_line: oauth2/apiKey · 3 schemes
tags:
- Company
- Business Applications
- Kubernetes
- Access Control
- Cloud Native Security
- Zero Trust
- DevSecOps
- IAM
- Open Source
---
