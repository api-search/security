---
anonymous_access: false
api_key_in: []
api_specs:
- filename: infranest-audit-log-api-openapi.yml
  format: yaml
  label: InfraNest Audit Log API
  slug: infranest-audit-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-audit-log-api-openapi.yml
- filename: infranest-authentication-api-openapi.yml
  format: yaml
  label: InfraNest Authentication API
  slug: infranest-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-authentication-api-openapi.yml
- filename: infranest-automations-api-openapi.yml
  format: yaml
  label: InfraNest Automations API
  slug: infranest-automations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-automations-api-openapi.yml
- filename: infranest-billing-api-openapi.yml
  format: yaml
  label: InfraNest Billing API
  slug: infranest-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-billing-api-openapi.yml
- filename: infranest-certificates-api-openapi.yml
  format: yaml
  label: InfraNest Certificates API
  slug: infranest-certificates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-certificates-api-openapi.yml
- filename: infranest-cloud-api-openapi.yml
  format: yaml
  label: InfraNest Cloud API
  slug: infranest-cloud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-cloud-api-openapi.yml
- filename: infranest-cost-api-openapi.yml
  format: yaml
  label: InfraNest Cost API
  slug: infranest-cost-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-cost-api-openapi.yml
- filename: infranest-cost-reporting-api-openapi.yml
  format: yaml
  label: InfraNest Cost reporting API
  slug: infranest-cost-reporting-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-cost-reporting-api-openapi.yml
- filename: infranest-custom-fields-api-openapi.yml
  format: yaml
  label: InfraNest Custom fields API
  slug: infranest-custom-fields-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-custom-fields-api-openapi.yml
- filename: infranest-dns-api-openapi.yml
  format: yaml
  label: InfraNest DNS API
  slug: infranest-dns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-dns-api-openapi.yml
- filename: infranest-domains-api-openapi.yml
  format: yaml
  label: InfraNest Domains API
  slug: infranest-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-domains-api-openapi.yml
- filename: infranest-drop-catch-api-openapi.yml
  format: yaml
  label: InfraNest Drop Catch API
  slug: infranest-drop-catch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-drop-catch-api-openapi.yml
- filename: infranest-dynamic-ip-api-openapi.yml
  format: yaml
  label: InfraNest Dynamic IP API
  slug: infranest-dynamic-ip-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-dynamic-ip-api-openapi.yml
- filename: infranest-endpoints-api-openapi.yml
  format: yaml
  label: InfraNest Endpoints API
  slug: infranest-endpoints-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-endpoints-api-openapi.yml
- filename: infranest-integration-logs-api-openapi.yml
  format: yaml
  label: InfraNest Integration Logs API
  slug: infranest-integration-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-integration-logs-api-openapi.yml
- filename: infranest-integrations-api-openapi.yml
  format: yaml
  label: InfraNest Integrations API
  slug: infranest-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-integrations-api-openapi.yml
- filename: infranest-monitoring-api-openapi.yml
  format: yaml
  label: InfraNest Monitoring API
  slug: infranest-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-monitoring-api-openapi.yml
- filename: infranest-organizations-api-openapi.yml
  format: yaml
  label: InfraNest Organizations API
  slug: infranest-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-organizations-api-openapi.yml
- filename: infranest-webhooks-api-openapi.yml
  format: yaml
  label: InfraNest Webhooks API
  slug: infranest-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/infranest/openapi/infranest-webhooks-api-openapi.yml
auth_types: []
description: InfraNest authentication methods
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Infranest Authentication
name_suffix: Authentication
oauth_flows: []
overview: InfraNest declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: InfraNest
provider_slug: infranest
scheme_count: 1
schemes:
- authorize_url: https://api.infranest.io/oauth/authorize
  evidence: 'InfraNest is an OAuth 2.1 authorization server: the authorization code flow with PKCE, and refresh tokens.'
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Obtain a client ID and register a redirect URI in the InfraNest developer console.
  name: InfraNest OAuth
  type: oauth2
slug: infranest-authentication
source_filename: infranest-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.infranest.io/oauth.md
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.infranest.io/oauth.md\nsources:\n- https://developers.infranest.io/oauth.md\n- https://infranest.io/docs/create-a-cloudflare-api-key/\n- https://infranest.io/docs/create-a-dynadot-api-key/\n- https://infranest.io/docs/create-a-godaddy-api-key/\ndescription: InfraNest authentication methods\nschemes:\n- type: oauth2\n  name: InfraNest OAuth\n  evidence: 'InfraNest is an OAuth 2.1 authorization server: the authorization code flow with PKCE, and refresh tokens.'\n  flows:\n  - authorization_code\n  - refresh_token\n  authorize_url: https://api.infranest.io/oauth/authorize\n  how_to_obtain: Obtain a client ID and register a redirect URI in the InfraNest developer console.\ndocs: https://developers.infranest.io/oauth.md\n"
source_yaml_url: https://artifacts.apis.io/infranest/authentication/infranest-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Infrastructure
- DNS
- Monitoring
- SSL
- Cloud
---
