---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: radiant-earth-accounts-api-openapi.yml
  format: yaml
  label: Radiant Earth Accounts API
  slug: radiant-earth-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radiant-earth/refs/heads/main/openapi/radiant-earth-accounts-api-openapi.yml
- filename: radiant-earth-api-keys-api-openapi.yml
  format: yaml
  label: Radiant Earth API Keys API
  slug: radiant-earth-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radiant-earth/refs/heads/main/openapi/radiant-earth-api-keys-api-openapi.yml
- filename: radiant-earth-authentication-api-openapi.yml
  format: yaml
  label: Radiant Earth Authentication API
  slug: radiant-earth-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radiant-earth/refs/heads/main/openapi/radiant-earth-authentication-api-openapi.yml
- filename: radiant-earth-data-connections-api-openapi.yml
  format: yaml
  label: Radiant Earth Data Connections API
  slug: radiant-earth-data-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radiant-earth/refs/heads/main/openapi/radiant-earth-data-connections-api-openapi.yml
- filename: radiant-earth-memberships-api-openapi.yml
  format: yaml
  label: Radiant Earth Memberships API
  slug: radiant-earth-memberships-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radiant-earth/refs/heads/main/openapi/radiant-earth-memberships-api-openapi.yml
- filename: radiant-earth-repositories-api-openapi.yml
  format: yaml
  label: Radiant Earth Repositories API
  slug: radiant-earth-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/radiant-earth/refs/heads/main/openapi/radiant-earth-repositories-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Radiant Earth Authentication
name_suffix: Authentication
oauth_flows: []
overview: Radiant Earth secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Radiant Earth
provider_slug: radiant-earth
scheme_count: 1
schemes:
- description: Follows the format `<access-key-id> <secret-access-key>`
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/radiant-earth-source-cooperative-openapi.yml
  type: apiKey
slug: radiant-earth-authentication
source_filename: radiant-earth-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: searched\nsource: https://docs.source.coop/automated-access\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Follows the format `<access-key-id> <secret-access-key>`\n  sources:\n  - openapi/radiant-earth-source-cooperative-openapi.yml\ndocs: https://docs.source.coop/automated-access\nadditional_mechanisms:\n- name: Service account API keys (data proxy)\n  description: An API key lets software sign in as a service account; AWS CLI/SDKs\n    trade the key at the data proxy STS endpoint (https://data.source.coop/.sts, AssumeRoleWithWebIdentity)\n    for credentials that last an hour. Keys must be sent in the request body, never\n    in a URL.\n  docs: https://docs.source.coop/automated-access\n- name: GitHub Actions OIDC\n  description: A service account can trust a GitHub Actions workflow, which signs\n    in with a token GitHub issues\
  \ for each run (no stored secret).\n  docs: https://docs.source.coop/automated-access\n- name: Interactive OIDC via Source CLI\n  description: source-coop login authenticates against the OIDC issuer https://auth.source.coop\n    (default scopes \"openid offline_access\") and caches short-lived credentials.\n  docs: https://github.com/source-cooperative/source-coop-cli\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/radiant-earth/refs/heads/main/authentication/radiant-earth-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Non-Profit
- Open Data
- Geospatial
- Earth Observation
- Cloud-Native Geospatial
- STAC
- Data Publishing
---
