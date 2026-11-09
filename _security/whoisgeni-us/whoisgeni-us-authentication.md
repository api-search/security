---
anonymous_access: false
api_key_in: []
api_specs:
- filename: whoisgeni-us-account-api-openapi.yml
  format: yaml
  label: whoisgeni-us Account API
  slug: whoisgeni-us-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-account-api-openapi.yml
- filename: whoisgeni-us-analysis-api-openapi.yml
  format: yaml
  label: whoisgeni-us Analysis API
  slug: whoisgeni-us-analysis-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-analysis-api-openapi.yml
- filename: whoisgeni-us-authentication-api-openapi.yml
  format: yaml
  label: whoisgeni-us Authentication API
  slug: whoisgeni-us-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-authentication-api-openapi.yml
- filename: whoisgeni-us-billing-api-openapi.yml
  format: yaml
  label: whoisgeni-us Billing API
  slug: whoisgeni-us-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-billing-api-openapi.yml
- filename: whoisgeni-us-byok-api-openapi.yml
  format: yaml
  label: whoisgeni-us Byok API
  slug: whoisgeni-us-byok-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-byok-api-openapi.yml
- filename: whoisgeni-us-correlation-api-openapi.yml
  format: yaml
  label: whoisgeni-us Correlation API
  slug: whoisgeni-us-correlation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-correlation-api-openapi.yml
- filename: whoisgeni-us-domains-api-openapi.yml
  format: yaml
  label: whoisgeni-us Domains API
  slug: whoisgeni-us-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-domains-api-openapi.yml
- filename: whoisgeni-us-entities-api-openapi.yml
  format: yaml
  label: whoisgeni-us Entities API
  slug: whoisgeni-us-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-entities-api-openapi.yml
- filename: whoisgeni-us-health-api-openapi.yml
  format: yaml
  label: whoisgeni-us Health API
  slug: whoisgeni-us-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-health-api-openapi.yml
- filename: whoisgeni-us-jobs-api-openapi.yml
  format: yaml
  label: whoisgeni-us Jobs API
  slug: whoisgeni-us-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-jobs-api-openapi.yml
- filename: whoisgeni-us-mcp-api-openapi.yml
  format: yaml
  label: whoisgeni-us MCP API
  slug: whoisgeni-us-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-mcp-api-openapi.yml
- filename: whoisgeni-us-schema-templates-api-openapi.yml
  format: yaml
  label: whoisgeni-us Schema Templates API
  slug: whoisgeni-us-schema-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-schema-templates-api-openapi.yml
- filename: whoisgeni-us-webhooks-api-openapi.yml
  format: yaml
  label: whoisgeni-us Webhooks API
  slug: whoisgeni-us-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/whoisgeni-us/openapi/whoisgeni-us-webhooks-api-openapi.yml
auth_types: []
description: These endpoints require a Cognito JWT token (Bearer authentication), not an API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Whoisgeni Us Authentication
name_suffix: Authentication
oauth_flows: []
overview: whoisgeni-us declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: whoisgeni-us
provider_slug: whoisgeni-us
scheme_count: 1
schemes:
- evidence: These endpoints require a Cognito JWT token (Bearer authentication), not an API key.
  header: Authorization
  how_to_obtain: Obtain a Cognito JWT token by signing in via the service's authentication flow.
  location: header
  name: Cognito JWT
  type: http-bearer
slug: whoisgeni-us-authentication
source_filename: whoisgeni-us-authentication.yml
source_heading: Authentication Profile
source_url: https://whoisgeni.us/api-reference/auth
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://whoisgeni.us/api-reference/auth\nsources:\n- https://whoisgeni.us/api-reference/auth\ndescription: These endpoints require a Cognito JWT token (Bearer authentication), not an API key.\nschemes:\n- type: http-bearer\n  name: Cognito JWT\n  evidence: These endpoints require a Cognito JWT token (Bearer authentication), not an API key.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a Cognito JWT token by signing in via the service's authentication flow.\ndocs: https://whoisgeni.us/api-reference/auth\n"
source_yaml_url: https://artifacts.apis.io/whoisgeni-us/authentication/whoisgeni-us-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Domain Intelligence
- Security
- Compliance
- Data Enrichment
---
