---
anonymous_access: false
api_key_in: []
api_specs:
- filename: leadfast-vip-matches-api-openapi.yml
  format: yaml
  label: LeadFast Matches API
  slug: leadfast-vip-matches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfast-vip/openapi/leadfast-vip-matches-api-openapi.yml
- filename: leadfast-vip-monitoring-api-openapi.yml
  format: yaml
  label: LeadFast Monitoring API
  slug: leadfast-vip-monitoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfast-vip/openapi/leadfast-vip-monitoring-api-openapi.yml
- filename: leadfast-vip-product-api-openapi.yml
  format: yaml
  label: LeadFast Product API
  slug: leadfast-vip-product-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/leadfast-vip/openapi/leadfast-vip-product-api-openapi.yml
auth_types: []
description: LeadFast API uses a bearer token passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: LeadFast Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeadFast declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LeadFast
provider_slug: leadfast-vip
scheme_count: 1
schemes:
- evidence: 'curl https://leadfast.vip/api/v1/matches?limit=5 \ -H "Authorization: Bearer $LEADFAST_API_KEY"'
  header: Authorization
  how_to_obtain: Create an API key in the LeadFast app under Integrations → API & agents and copy the secret.
  location: header
  name: Bearer
  type: http-bearer
slug: leadfast-vip-authentication
source_filename: leadfast-vip-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.leadfast.vip/quickstart.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.leadfast.vip/quickstart.md\nsources:\n- https://docs.leadfast.vip/quickstart.md\n- https://docs.leadfast.vip/quickstart\ndescription: LeadFast API uses a bearer token passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'curl https://leadfast.vip/api/v1/matches?limit=5 \\ -H \"Authorization: Bearer $LEADFAST_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the LeadFast app under Integrations → API & agents and copy the secret.\nnote: No OAuth2, apiKey, or other authentication schemes are documented.\ndocs: https://docs.leadfast.vip/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/leadfast-vip/authentication/leadfast-vip-authentication.yml
summary_line: 1 scheme
tags:
- Lead Generation
- Reddit Monitoring
- Software-as-a-Service
- Developer Tools
- Home Automation
- Marketing Automation
---
