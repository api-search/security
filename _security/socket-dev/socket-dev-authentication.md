---
api_key_in: []
api_specs:
- filename: socket-packages-api-openapi.yml
  format: yaml
  label: Socket Packages API
  slug: socket-packages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-packages-api-openapi.yml
- filename: socket-full-scans-api-openapi.yml
  format: yaml
  label: Socket Full Scans API
  slug: socket-full-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-full-scans-api-openapi.yml
- filename: socket-diff-scans-api-openapi.yml
  format: yaml
  label: Socket Diff Scans API
  slug: socket-diff-scans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-diff-scans-api-openapi.yml
- filename: socket-alerts-api-openapi.yml
  format: yaml
  label: Socket Alerts API
  slug: socket-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-alerts-api-openapi.yml
- filename: socket-triage-api-openapi.yml
  format: yaml
  label: Socket Triage API
  slug: socket-triage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-triage-api-openapi.yml
- filename: socket-repos-api-openapi.yml
  format: yaml
  label: Socket Repos API
  slug: socket-repos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-repos-api-openapi.yml
- filename: socket-org-settings-api-openapi.yml
  format: yaml
  label: Socket Organization Settings API
  slug: socket-org-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-org-settings-api-openapi.yml
- filename: socket-webhooks-api-openapi.yml
  format: yaml
  label: Socket Webhooks API
  slug: socket-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-webhooks-api-openapi.yml
- filename: socket-threat-feed-api-openapi.yml
  format: yaml
  label: Socket Threat Feed API
  slug: socket-threat-feed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-threat-feed-api-openapi.yml
- filename: socket-fixes-api-openapi.yml
  format: yaml
  label: Socket Fixes API
  slug: socket-fixes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-fixes-api-openapi.yml
- filename: socket-dependencies-api-openapi.yml
  format: yaml
  label: Socket Dependencies API
  slug: socket-dependencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-dependencies-api-openapi.yml
- filename: socket-api-tokens-api-openapi.yml
  format: yaml
  label: Socket API Tokens API
  slug: socket-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-api-tokens-api-openapi.yml
- filename: socket-audit-log-api-openapi.yml
  format: yaml
  label: Socket Audit Log API
  slug: socket-audit-log-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-audit-log-api-openapi.yml
- filename: socket-org-snapshots-api-openapi.yml
  format: yaml
  label: Socket Organization Snapshots API
  slug: socket-org-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-org-snapshots-api-openapi.yml
- filename: socket-metadata-api-openapi.yml
  format: yaml
  label: Socket Metadata API
  slug: socket-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/openapi/socket-metadata-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Socket Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Socket secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Socket
provider_slug: socket-dev
scheme_count: 2
schemes:
- description: Organization Tokens can be passed as a Bearer token
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/socket-alerts-api-openapi.yml
  - openapi/socket-api-tokens-api-openapi.yml
  - openapi/socket-audit-log-api-openapi.yml
  - openapi/socket-dependencies-api-openapi.yml
  - openapi/socket-diff-scans-api-openapi.yml
  - openapi/socket-fixes-api-openapi.yml
  - openapi/socket-full-scans-api-openapi.yml
  - openapi/socket-metadata-api-openapi.yml
  - openapi/socket-org-settings-api-openapi.yml
  - openapi/socket-org-snapshots-api-openapi.yml
  - openapi/socket-packages-api-openapi.yml
  - openapi/socket-repos-api-openapi.yml
  - openapi/socket-threat-feed-api-openapi.yml
  - openapi/socket-triage-api-openapi.yml
  - openapi/socket-webhooks-api-openapi.yml
  type: http
- description: Organization Tokens can be passed as the user field in basic auth
  name: basicAuth
  scheme: basic
  sources:
  - openapi/socket-alerts-api-openapi.yml
  - openapi/socket-api-tokens-api-openapi.yml
  - openapi/socket-audit-log-api-openapi.yml
  - openapi/socket-dependencies-api-openapi.yml
  - openapi/socket-diff-scans-api-openapi.yml
  - openapi/socket-fixes-api-openapi.yml
  - openapi/socket-full-scans-api-openapi.yml
  - openapi/socket-metadata-api-openapi.yml
  - openapi/socket-org-settings-api-openapi.yml
  - openapi/socket-org-snapshots-api-openapi.yml
  - openapi/socket-packages-api-openapi.yml
  - openapi/socket-repos-api-openapi.yml
  - openapi/socket-threat-feed-api-openapi.yml
  - openapi/socket-triage-api-openapi.yml
  - openapi/socket-webhooks-api-openapi.yml
  type: http
slug: socket-dev-authentication
source_filename: socket-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/socket-alerts-api-openapi.yml, openapi/socket-api-tokens-api-openapi.yml, openapi/socket-audit-log-api-openapi.yml,\n  openapi/socket-dependencies-api-openapi.yml, openapi/socket-diff-scans-api-openapi.yml, openapi/socket-fixes-api-openapi.yml,\n  openapi/socket-full-scans-api-openapi.yml, openapi/socket-metadata-api-openapi.yml, openapi/socket-org-settings-api-openapi.yml,\n  openapi/socket-org-snapshots-api-openapi.yml, openapi/socket-packages-api-openapi.yml, openapi/socket-repos-api-openapi.yml\n  ...\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Organization Tokens can be passed as a Bearer token\n  sources:\n  - openapi/socket-alerts-api-openapi.yml\n  - openapi/socket-api-tokens-api-openapi.yml\n  - openapi/socket-audit-log-api-openapi.yml\n  - openapi/socket-dependencies-api-openapi.yml\n  - openapi/socket-diff-scans-api-openapi.yml\n  - openapi/socket-fixes-api-openapi.yml\n\
  \  - openapi/socket-full-scans-api-openapi.yml\n  - openapi/socket-metadata-api-openapi.yml\n  - openapi/socket-org-settings-api-openapi.yml\n  - openapi/socket-org-snapshots-api-openapi.yml\n  - openapi/socket-packages-api-openapi.yml\n  - openapi/socket-repos-api-openapi.yml\n  - openapi/socket-threat-feed-api-openapi.yml\n  - openapi/socket-triage-api-openapi.yml\n  - openapi/socket-webhooks-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Organization Tokens can be passed as the user field in basic auth\n  sources:\n  - openapi/socket-alerts-api-openapi.yml\n  - openapi/socket-api-tokens-api-openapi.yml\n  - openapi/socket-audit-log-api-openapi.yml\n  - openapi/socket-dependencies-api-openapi.yml\n  - openapi/socket-diff-scans-api-openapi.yml\n  - openapi/socket-fixes-api-openapi.yml\n  - openapi/socket-full-scans-api-openapi.yml\n  - openapi/socket-metadata-api-openapi.yml\n  - openapi/socket-org-settings-api-openapi.yml\n  - openapi/socket-org-snapshots-api-openapi.yml\n\
  \  - openapi/socket-packages-api-openapi.yml\n  - openapi/socket-repos-api-openapi.yml\n  - openapi/socket-threat-feed-api-openapi.yml\n  - openapi/socket-triage-api-openapi.yml\n  - openapi/socket-webhooks-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/socket-dev/refs/heads/main/authentication/socket-dev-authentication.yml
summary_line: http · 2 schemes
tags:
- Supply Chain Security
- Open Source Security
- Software Composition Analysis
- SCA
- Malware Detection
- Dependency Scanning
- SBOM
- npm
- PyPI
- Go
- Maven
- Cargo
- NuGet
- RubyGems
- Developer Security
---
