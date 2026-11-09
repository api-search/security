---
anonymous_access: false
api_key_in: []
api_specs:
- filename: prospectapis-pricing-api-openapi.yml
  format: yaml
  label: ProspectAPIs Pricing API
  slug: prospectapis-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-pricing-api-openapi.yml
- filename: prospectapis-watchlists-api-openapi.yml
  format: yaml
  label: ProspectAPIs Watchlists API
  slug: prospectapis-watchlists-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-watchlists-api-openapi.yml
- filename: prospectapis-account-api-openapi.yml
  format: yaml
  label: ProspectAPIs Account API
  slug: prospectapis-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-account-api-openapi.yml
- filename: prospectapis-account-insights-api-openapi.yml
  format: yaml
  label: ProspectAPIs Account insights API
  slug: prospectapis-account-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-account-insights-api-openapi.yml
- filename: prospectapis-ads-api-openapi.yml
  format: yaml
  label: ProspectAPIs Ads API
  slug: prospectapis-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-ads-api-openapi.yml
- filename: prospectapis-companies-api-openapi.yml
  format: yaml
  label: ProspectAPIs Companies API
  slug: prospectapis-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-companies-api-openapi.yml
- filename: prospectapis-connected-account-api-openapi.yml
  format: yaml
  label: ProspectAPIs Connected account API
  slug: prospectapis-connected-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-connected-account-api-openapi.yml
- filename: prospectapis-email-verification-api-openapi.yml
  format: yaml
  label: ProspectAPIs Email verification API
  slug: prospectapis-email-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-email-verification-api-openapi.yml
- filename: prospectapis-events-api-openapi.yml
  format: yaml
  label: ProspectAPIs Events API
  slug: prospectapis-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-events-api-openapi.yml
- filename: prospectapis-funding-api-openapi.yml
  format: yaml
  label: ProspectAPIs Funding API
  slug: prospectapis-funding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-funding-api-openapi.yml
- filename: prospectapis-health-api-openapi.yml
  format: yaml
  label: ProspectAPIs Health API
  slug: prospectapis-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-health-api-openapi.yml
- filename: prospectapis-launches-api-openapi.yml
  format: yaml
  label: ProspectAPIs Launches API
  slug: prospectapis-launches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-launches-api-openapi.yml
- filename: prospectapis-messaging-reads-api-openapi.yml
  format: yaml
  label: ProspectAPIs Messaging reads API
  slug: prospectapis-messaging-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-messaging-reads-api-openapi.yml
- filename: prospectapis-meta-api-openapi.yml
  format: yaml
  label: ProspectAPIs Meta API
  slug: prospectapis-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-meta-api-openapi.yml
- filename: prospectapis-people-reads-api-openapi.yml
  format: yaml
  label: ProspectAPIs People reads API
  slug: prospectapis-people-reads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-people-reads-api-openapi.yml
- filename: prospectapis-people-writes-api-openapi.yml
  format: yaml
  label: ProspectAPIs People writes API
  slug: prospectapis-people-writes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-people-writes-api-openapi.yml
- filename: prospectapis-prospectapis-api-api-openapi.yml
  format: yaml
  label: ProspectAPIs ProspectAPIs API
  slug: prospectapis-prospectapis-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-prospectapis-api-api-openapi.yml
- filename: prospectapis-research-api-openapi.yml
  format: yaml
  label: ProspectAPIs Research API
  slug: prospectapis-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/prospectapis/openapi/prospectapis-research-api-openapi.yml
auth_types: []
description: Authentication schemes for ProspectAPIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Prospectapis Authentication
name_suffix: Authentication
oauth_flows: []
overview: ProspectAPIs declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ProspectAPIs
provider_slug: prospectapis
scheme_count: 2
schemes:
- evidence: ProspectAPIs API authentication is a secret API key sent as a Bearer token in the Authorization header of every /v1 request.
  name: Authorization
  type: apiKey
- evidence: Clients that support remote servers can instead sign in with OAuth , and the connected app then shows in your key list
  name: OAuth
  type: oauth2
slug: prospectapis-authentication
source_filename: prospectapis-authentication.yml
source_heading: Authentication Profile
source_url: https://prospectapis.com/docs/authentication
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://prospectapis.com/docs/authentication\nsources:\n- https://prospectapis.com/docs/authentication\n- https://prospectapis.com/mcp#oauth\n- https://prospectapis.com/docs/reference/connect-account-login\n- https://prospectapis.com/faq#getting-started\ndescription: Authentication schemes for ProspectAPIs\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: ProspectAPIs API authentication is a secret API key sent as a Bearer token in the Authorization header of every /v1 request.\n- type: oauth2\n  name: OAuth\n  evidence: Clients that support remote servers can instead sign in with OAuth , and the connected app then shows in your key list\ndocs: https://prospectapis.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/prospectapis/authentication/prospectapis-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Funding
- Research
- Data
- Funding Data
- Prospect Research
- Email Verification
- LinkedIn data
- Watchlist
- MCP
---
