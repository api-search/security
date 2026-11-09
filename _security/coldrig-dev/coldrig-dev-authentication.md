---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coldrig-dev-account-api-openapi.yml
  format: yaml
  label: Coldrig Account API
  slug: coldrig-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-account-api-openapi.yml
- filename: coldrig-dev-bootstrap-api-openapi.yml
  format: yaml
  label: Coldrig Bootstrap API
  slug: coldrig-dev-bootstrap-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-bootstrap-api-openapi.yml
- filename: coldrig-dev-byo-domains-api-openapi.yml
  format: yaml
  label: Coldrig Byo Domains API
  slug: coldrig-dev-byo-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-byo-domains-api-openapi.yml
- filename: coldrig-dev-campaigns-api-openapi.yml
  format: yaml
  label: Coldrig Campaigns API
  slug: coldrig-dev-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-campaigns-api-openapi.yml
- filename: coldrig-dev-compliance-api-openapi.yml
  format: yaml
  label: Coldrig Compliance API
  slug: coldrig-dev-compliance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-compliance-api-openapi.yml
- filename: coldrig-dev-dashboard-api-openapi.yml
  format: yaml
  label: Coldrig Dashboard API
  slug: coldrig-dev-dashboard-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-dashboard-api-openapi.yml
- filename: coldrig-dev-inbox-api-openapi.yml
  format: yaml
  label: Coldrig Inbox API
  slug: coldrig-dev-inbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-inbox-api-openapi.yml
- filename: coldrig-dev-infrastructure-api-openapi.yml
  format: yaml
  label: Coldrig Infrastructure API
  slug: coldrig-dev-infrastructure-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-infrastructure-api-openapi.yml
- filename: coldrig-dev-leads-api-openapi.yml
  format: yaml
  label: Coldrig Leads API
  slug: coldrig-dev-leads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-leads-api-openapi.yml
- filename: coldrig-dev-messages-api-openapi.yml
  format: yaml
  label: Coldrig Messages API
  slug: coldrig-dev-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-messages-api-openapi.yml
- filename: coldrig-dev-sandbox-api-openapi.yml
  format: yaml
  label: Coldrig Sandbox API
  slug: coldrig-dev-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-sandbox-api-openapi.yml
- filename: coldrig-dev-webhooks-api-openapi.yml
  format: yaml
  label: Coldrig Webhooks API
  slug: coldrig-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/coldrig-dev/openapi/coldrig-dev-webhooks-api-openapi.yml
auth_types: []
description: ColdRig authentication methods as described on the Connect page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Coldrig Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coldrig declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Coldrig
provider_slug: coldrig-dev
scheme_count: 2
schemes:
- evidence: Sign-in is OAuth, and your user presses Allow themselves.
  how_to_obtain: User signs in via browser and presses Allow; the service returns an access token used as a Bearer token.
  name: OAuth
  type: oauth2
- evidence: 'If sign-in fails, tell your user to set COLDRIG_TOKEN to their API key in their own terminal and send it as the header "Authorization: Bearer $COLDRIG_TOKEN".'
  header: Authorization
  how_to_obtain: User obtains an API key from Coldrig and sets it in the COLDRIG_TOKEN environment variable, which is then sent as a Bearer token in the Authorization header.
  location: header
  name: API Key Bearer Token
  type: http-bearer
slug: coldrig-dev-authentication
source_filename: coldrig-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://coldrig.dev/connect
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://coldrig.dev/connect\nsources:\n- https://coldrig.dev/connect\ndescription: ColdRig authentication methods as described on the Connect page.\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: Sign-in is OAuth, and your user presses Allow themselves.\n  how_to_obtain: User signs in via browser and presses Allow; the service returns an access token used as a Bearer token.\n- type: http-bearer\n  name: API Key Bearer Token\n  evidence: 'If sign-in fails, tell your user to set COLDRIG_TOKEN to their API key in their own terminal and send it as the header \"Authorization:\n    Bearer $COLDRIG_TOKEN\".'\n  location: header\n  header: Authorization\n  how_to_obtain: User obtains an API key from Coldrig and sets it in the COLDRIG_TOKEN environment variable, which is then sent as a Bearer token\n    in the Authorization header.\ndocs: https://coldrig.dev/connect\n"
source_yaml_url: https://artifacts.apis.io/coldrig-dev/authentication/coldrig-dev-authentication.yml
summary_line: 2 schemes
tags:
- Cold Email
- Outreach
- AI Agents
- Email Infrastructure
---
