---
anonymous_access: false
api_key_in: []
api_specs:
- filename: piwik-pro-access-control-api-openapi.yml
  format: yaml
  label: Piwik PRO Access Control API
  slug: piwik-pro-access-control-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-access-control-api-openapi.yml
- filename: piwik-pro-analytics-api-openapi.yml
  format: yaml
  label: Piwik PRO Analytics API
  slug: piwik-pro-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-analytics-api-openapi.yml
- filename: piwik-pro-apps-api-openapi.yml
  format: yaml
  label: Piwik PRO Apps API
  slug: piwik-pro-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-apps-api-openapi.yml
- filename: piwik-pro-audit-log-api-openapi.yml
  format: yaml
  label: Piwik PRO Audit Log API
  slug: piwik-pro-audit-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-audit-log-api-openapi.yml
- filename: piwik-pro-container-settings-api-openapi.yml
  format: yaml
  label: Piwik PRO Container Settings API
  slug: piwik-pro-container-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-container-settings-api-openapi.yml
- filename: piwik-pro-data-activation-api-openapi.yml
  format: yaml
  label: Piwik PRO Data Activation API
  slug: piwik-pro-data-activation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-data-activation-api-openapi.yml
- filename: piwik-pro-meta-sites-api-openapi.yml
  format: yaml
  label: Piwik PRO Meta sites API
  slug: piwik-pro-meta-sites-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-meta-sites-api-openapi.yml
- filename: piwik-pro-modules-api-openapi.yml
  format: yaml
  label: Piwik PRO Modules API
  slug: piwik-pro-modules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-modules-api-openapi.yml
- filename: piwik-pro-oauth-api-openapi.yml
  format: yaml
  label: Piwik PRO OAuth API
  slug: piwik-pro-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-oauth-api-openapi.yml
- filename: piwik-pro-tag-manager-api-openapi.yml
  format: yaml
  label: Piwik PRO Tag Manager API
  slug: piwik-pro-tag-manager-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-tag-manager-api-openapi.yml
- filename: piwik-pro-tracker-api-openapi.yml
  format: yaml
  label: Piwik PRO Tracker API
  slug: piwik-pro-tracker-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-tracker-api-openapi.yml
- filename: piwik-pro-tracker-settings-api-openapi.yml
  format: yaml
  label: Piwik PRO Tracker Settings API
  slug: piwik-pro-tracker-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-tracker-settings-api-openapi.yml
- filename: piwik-pro-user-groups-api-openapi.yml
  format: yaml
  label: Piwik PRO User Groups API
  slug: piwik-pro-user-groups-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-user-groups-api-openapi.yml
- filename: piwik-pro-users-api-openapi.yml
  format: yaml
  label: Piwik PRO Users API
  slug: piwik-pro-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/piwik-pro/openapi/piwik-pro-users-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Piwik PRO Authentication
name_suffix: Authentication
oauth_flows: []
overview: Piwik PRO declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Piwik PRO
provider_slug: piwik-pro
scheme_count: 1
schemes:
- evidence: Our API uses client credentials (OAuth grant type) for obtaining a user token.
  header: Authorization
  how_to_obtain: Create API keys in the Piwik PRO UI to get a Client ID and Client secret, then POST to the token endpoint with grant_type client_credentials.
  location: header
  name: OAuth2 Client Credentials
  token_url: https://{account}.piwik.pro/auth/token
  type: http-bearer
slug: piwik-pro-authentication
source_filename: piwik-pro-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.piwik.pro/reference/authentication.md
source_yaml: "generated: '2026-11-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.piwik.pro/reference/authentication.md\nsources:\n- https://developers.piwik.pro/reference/authentication.md\n- https://developers.piwik.pro/reference/oauth_token_issue.md\n- https://developers.piwik.pro/reference/authentication\n- https://developers.piwik.pro/docs/browser-js-api.md\nschemes:\n- type: http-bearer\n  name: OAuth2 Client Credentials\n  evidence: Our API uses client credentials (OAuth grant type) for obtaining a user token.\n  location: header\n  header: Authorization\n  token_url: https://{account}.piwik.pro/auth/token\n  how_to_obtain: Create API keys in the Piwik PRO UI to get a Client ID and Client secret, then POST to the token endpoint with grant_type client_credentials.\ndocs: https://developers.piwik.pro/reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/piwik-pro/authentication/piwik-pro-authentication.yml
summary_line: 1 scheme
tags:
- Analytics
- Privacy
- Data Activation
- Enterprise
- Compliance
---
