---
api_key_in: []
api_specs:
- filename: socket-alerts-api-openapi.yml
  format: yaml
  label: Socket alerts API
  slug: socket-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-alerts-api-openapi.yml
- filename: socket-api-tokens-api-openapi.yml
  format: yaml
  label: Socket api-tokens API
  slug: socket-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-api-tokens-api-openapi.yml
- filename: socket-audit-log-api-openapi.yml
  format: yaml
  label: Socket audit-log API
  slug: socket-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-audit-log-api-openapi.yml
- filename: socket-dependencies-api-openapi.yml
  format: yaml
  label: Socket dependencies API
  slug: socket-dependencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-dependencies-api-openapi.yml
- filename: socket-deprecated-api-openapi.yml
  format: yaml
  label: Socket deprecated API
  slug: socket-deprecated-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-deprecated-api-openapi.yml
- filename: socket-diff-scans-api-openapi.yml
  format: yaml
  label: Socket diff-scans API
  slug: socket-diff-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-diff-scans-api-openapi.yml
- filename: socket-fixes-api-openapi.yml
  format: yaml
  label: Socket fixes API
  slug: socket-fixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-fixes-api-openapi.yml
- filename: socket-full-scans-api-openapi.yml
  format: yaml
  label: Socket full-scans API
  slug: socket-full-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-full-scans-api-openapi.yml
- filename: socket-license-policy-api-openapi.yml
  format: yaml
  label: Socket license-policy API
  slug: socket-license-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-license-policy-api-openapi.yml
- filename: socket-metadata-api-openapi.yml
  format: yaml
  label: Socket metadata API
  slug: socket-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-metadata-api-openapi.yml
- filename: socket-org-settings-api-openapi.yml
  format: yaml
  label: Socket org-settings API
  slug: socket-org-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-org-settings-api-openapi.yml
- filename: socket-org-snapshots-api-openapi.yml
  format: yaml
  label: Socket org-snapshots API
  slug: socket-org-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-org-snapshots-api-openapi.yml
- filename: socket-packages-api-openapi.yml
  format: yaml
  label: Socket packages API
  slug: socket-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-packages-api-openapi.yml
- filename: socket-repo-labels-api-openapi.yml
  format: yaml
  label: Socket repo-labels API
  slug: socket-repo-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-repo-labels-api-openapi.yml
- filename: socket-repos-api-openapi.yml
  format: yaml
  label: Socket repos API
  slug: socket-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-repos-api-openapi.yml
- filename: socket-security-policy-api-openapi.yml
  format: yaml
  label: Socket security-policy API
  slug: socket-security-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-security-policy-api-openapi.yml
- filename: socket-telemetry-api-openapi.yml
  format: yaml
  label: Socket telemetry API
  slug: socket-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-telemetry-api-openapi.yml
- filename: socket-threat-feed-api-openapi.yml
  format: yaml
  label: Socket threat-feed API
  slug: socket-threat-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-threat-feed-api-openapi.yml
- filename: socket-triage-api-openapi.yml
  format: yaml
  label: Socket triage API
  slug: socket-triage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-triage-api-openapi.yml
- filename: socket-webhooks-api-openapi.yml
  format: yaml
  label: Socket webhooks API
  slug: socket-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/openapi/socket-webhooks-api-openapi.yml
auth_types:
- http
description: 'Socket authenticates REST API requests with an organization API token. The OpenAPI declares two HTTP schemes: bearer and basic. The same token is used either as an Authorization Bearer credential or as the Basic-auth username (with an empty password). Tokens carry fine-grained scopes (see scopes/socket-scopes.yml) and are metered by quota.'
kind: authentication
layout: security
method: searched
name: Socket Authentication
name_suffix: Authentication
oauth_flows: []
overview: Socket secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Socket
provider_slug: socket
scheme_count: 2
schemes:
- description: 'Authorization: Bearer <ORG_API_TOKEN>'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/socket-openapi-original.json
  type: http
- description: HTTP Basic with the API token as the username and an empty password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/socket-openapi-original.json
  type: http
slug: socket-authentication
source_filename: socket-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/socket-openapi-original.json\ndocs: https://docs.socket.dev/reference/authentication\ndescription: >-\n  Socket authenticates REST API requests with an organization API token. The OpenAPI declares\n  two HTTP schemes: bearer and basic. The same token is used either as an Authorization Bearer\n  credential or as the Basic-auth username (with an empty password). Tokens carry fine-grained\n  scopes (see scopes/socket-scopes.yml) and are metered by quota.\nsummary:\n  types: [http]\n  http_schemes: [bearer, basic]\n  api_key_in: []\n  oauth2_flows: []\n  token_scopes: true\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer <ORG_API_TOKEN>'\n  sources: [openapi/socket-openapi-original.json]\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic with the API token as the username and an empty password.\n  sources: [openapi/socket-openapi-original.json]\n\
  token_management:\n  docs: https://docs.socket.dev/reference/creating-and-managing-api-tokens\n  operations: [postAPIToken, getAPITokens, postAPITokenUpdate, postAPITokensRotate, postAPITokensRevoke]\n  scopes_artifact: scopes/socket-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socket/refs/heads/main/authentication/socket-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Security
- Software Supply Chain Security
- Dependency Scanning
- Software Composition Analysis
- Vulnerability Management
- Open Source Security
- DevSecOps
- SBOM
- Package Analysis
---
