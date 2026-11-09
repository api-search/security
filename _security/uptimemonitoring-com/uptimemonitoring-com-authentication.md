---
anonymous_access: false
api_key_in: []
api_specs:
- filename: uptimemonitoring-com-account-api-openapi.yml
  format: yaml
  label: Monitive Account API
  slug: uptimemonitoring-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-account-api-openapi.yml
- filename: uptimemonitoring-com-admin-api-openapi.yml
  format: yaml
  label: Monitive Admin API
  slug: uptimemonitoring-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-admin-api-openapi.yml
- filename: uptimemonitoring-com-announcements-api-openapi.yml
  format: yaml
  label: Monitive Announcements API
  slug: uptimemonitoring-com-announcements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-announcements-api-openapi.yml
- filename: uptimemonitoring-com-email-api-openapi.yml
  format: yaml
  label: Monitive Email API
  slug: uptimemonitoring-com-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-email-api-openapi.yml
- filename: uptimemonitoring-com-events-api-openapi.yml
  format: yaml
  label: Monitive Events API
  slug: uptimemonitoring-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-events-api-openapi.yml
- filename: uptimemonitoring-com-feed-api-openapi.yml
  format: yaml
  label: Monitive Feed API
  slug: uptimemonitoring-com-feed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-feed-api-openapi.yml
- filename: uptimemonitoring-com-feed-xml-api-openapi.yml
  format: yaml
  label: Monitive Feed.xml API
  slug: uptimemonitoring-com-feed-xml-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-feed-xml-api-openapi.yml
- filename: uptimemonitoring-com-incidents-api-openapi.yml
  format: yaml
  label: Monitive Incidents API
  slug: uptimemonitoring-com-incidents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-incidents-api-openapi.yml
- filename: uptimemonitoring-com-keys-api-openapi.yml
  format: yaml
  label: Monitive Keys API
  slug: uptimemonitoring-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-keys-api-openapi.yml
- filename: uptimemonitoring-com-monitors-api-openapi.yml
  format: yaml
  label: Monitive Monitors API
  slug: uptimemonitoring-com-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-monitors-api-openapi.yml
- filename: uptimemonitoring-com-oauth-api-openapi.yml
  format: yaml
  label: Monitive OAuth API
  slug: uptimemonitoring-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-oauth-api-openapi.yml
- filename: uptimemonitoring-com-public-api-openapi.yml
  format: yaml
  label: Monitive Public API
  slug: uptimemonitoring-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-public-api-openapi.yml
- filename: uptimemonitoring-com-push-api-openapi.yml
  format: yaml
  label: Monitive Push API
  slug: uptimemonitoring-com-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-push-api-openapi.yml
- filename: uptimemonitoring-com-recipients-api-openapi.yml
  format: yaml
  label: Monitive Recipients API
  slug: uptimemonitoring-com-recipients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-recipients-api-openapi.yml
- filename: uptimemonitoring-com-webhook-deliveries-api-openapi.yml
  format: yaml
  label: Monitive Webhook Deliveries API
  slug: uptimemonitoring-com-webhook-deliveries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptimemonitoring-com/openapi/uptimemonitoring-com-webhook-deliveries-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Uptimemonitoring Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Monitive declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Monitive
provider_slug: uptimemonitoring-com
scheme_count: 2
schemes:
- description: GitHub and Google OAuth sign‑in flows.
  flows:
    authorizationCode:
      authorizationUrl: https://app.uptimemonitoring.com/oauth/authorize
      tokenUrl: https://app.uptimemonitoring.com/oauth/token
  type: oauth2
- description: Bearer token with `umk_live_` prefix.
  format: Bearer
  in: header
  name: Authorization
  rotation:
    grace_window: 5 minutes
    max_keys: 10
  type: apiKey
slug: uptimemonitoring-com-authentication
source_filename: uptimemonitoring-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://uptimemonitoring.com/docs/authentication.md\nschemes:\n  - type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://app.uptimemonitoring.com/oauth/authorize\n        tokenUrl: https://app.uptimemonitoring.com/oauth/token\n    description: GitHub and Google OAuth sign‑in flows.\n  - type: apiKey\n    name: Authorization\n    in: header\n    description: Bearer token with `umk_live_` prefix.\n    format: Bearer\n    rotation:\n      max_keys: 10\n      grace_window: 5 minutes\n"
source_yaml_url: https://artifacts.apis.io/uptimemonitoring-com/authentication/uptimemonitoring-com-authentication.yml
summary_line: 2 schemes
tags:
- Uptime Monitoring
- API-First
- Developer Tools
- Observability
- Software-as-a-Service
---
