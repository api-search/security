---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jobopportunitiesapi-org-companies-api-openapi.yml
  format: yaml
  label: jobopportunitiesapi-org Companies API
  slug: jobopportunitiesapi-org-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobopportunitiesapi-org/openapi/jobopportunitiesapi-org-companies-api-openapi.yml
- filename: jobopportunitiesapi-org-jobs-api-openapi.yml
  format: yaml
  label: jobopportunitiesapi-org Jobs API
  slug: jobopportunitiesapi-org-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobopportunitiesapi-org/openapi/jobopportunitiesapi-org-jobs-api-openapi.yml
- filename: jobopportunitiesapi-org-meta-api-openapi.yml
  format: yaml
  label: jobopportunitiesapi-org Meta API
  slug: jobopportunitiesapi-org-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobopportunitiesapi-org/openapi/jobopportunitiesapi-org-meta-api-openapi.yml
- filename: jobopportunitiesapi-org-public-api-openapi.yml
  format: yaml
  label: jobopportunitiesapi-org Public API
  slug: jobopportunitiesapi-org-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobopportunitiesapi-org/openapi/jobopportunitiesapi-org-public-api-openapi.yml
auth_types: []
description: Authentication is performed by sending the secret key as a bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Jobopportunitiesapi Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: jobopportunitiesapi-org declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: jobopportunitiesapi-org
provider_slug: jobopportunitiesapi-org
scheme_count: 1
schemes:
- evidence: 'The header § Authorization: Bearer <your key>, on every /v1 request — and on the four /public listing routes too'
  header: Authorization
  how_to_obtain: Create a free key on the dashboard; the secret is shown once when the key is created.
  location: header
  name: Bearer
  type: http-bearer
slug: jobopportunitiesapi-org-authentication
source_filename: jobopportunitiesapi-org-authentication.yml
source_heading: Authentication Profile
source_url: https://jobopportunitiesapi.org/docs/api/authentication
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://jobopportunitiesapi.org/docs/api/authentication\nsources:\n- https://jobopportunitiesapi.org/docs/api/authentication\n- https://jobopportunitiesapi.org/docs/quickstart\n- https://jobopportunitiesapi.org/docs/ai/quickstart.md\ndescription: Authentication is performed by sending the secret key as a bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'The header § Authorization: Bearer <your key>, on every /v1 request — and on the four /public listing routes too'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a free key on the dashboard; the secret is shown once when the key is created.\nnote: No OAuth flows, apiKey, or other authentication methods are documented.\ndocs: https://jobopportunitiesapi.org/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/jobopportunitiesapi-org/authentication/jobopportunitiesapi-org-authentication.yml
summary_line: 1 scheme
tags:
- Job
- Employment Data
- Data Provenance
- Job Board
- AI Agents
---
