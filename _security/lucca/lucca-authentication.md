---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lucca-employee-attributes-api-openapi.yml
  format: yaml
  label: Lucca Employee Attributes API
  slug: lucca-employee-attributes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employee-attributes-api-openapi.yml
- filename: lucca-employee-job-qualifications-api-openapi.yml
  format: yaml
  label: Lucca Employee Job Qualifications API
  slug: lucca-employee-job-qualifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employee-job-qualifications-api-openapi.yml
- filename: lucca-employee-occupation-categories-api-openapi.yml
  format: yaml
  label: Lucca Employee Occupation Categories API
  slug: lucca-employee-occupation-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employee-occupation-categories-api-openapi.yml
- filename: lucca-employees-api-openapi.yml
  format: yaml
  label: Lucca Employees API
  slug: lucca-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employees-api-openapi.yml
- filename: lucca-employments-api-openapi.yml
  format: yaml
  label: Lucca Employments API
  slug: lucca-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-employments-api-openapi.yml
- filename: lucca-events-api-openapi.yml
  format: yaml
  label: Lucca Events API
  slug: lucca-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-events-api-openapi.yml
- filename: lucca-files-api-openapi.yml
  format: yaml
  label: Lucca Files API
  slug: lucca-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-files-api-openapi.yml
- filename: lucca-organization-api-openapi.yml
  format: yaml
  label: Lucca Organization API
  slug: lucca-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-organization-api-openapi.yml
- filename: lucca-taxonomies-api-openapi.yml
  format: yaml
  label: Lucca Taxonomies API
  slug: lucca-taxonomies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-taxonomies-api-openapi.yml
- filename: lucca-webhooks-api-openapi.yml
  format: yaml
  label: Lucca Webhooks API
  slug: lucca-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-webhooks-api-openapi.yml
- filename: lucca-working-time-arrangements-api-openapi.yml
  format: yaml
  label: Lucca Working Time Arrangements API
  slug: lucca-working-time-arrangements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/openapi/lucca-working-time-arrangements-api-openapi.yml
auth_types: []
description: 'Lucca supports two authentication methods: an API key for the Legacy API and OAuth2 client credentials for the current API.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Lucca Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lucca declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Lucca
provider_slug: lucca
scheme_count: 1
schemes:
- evidence: 'Once you have an API key, you must reference it on all requests against the Legacy APIs through the `Authorization` HTTP header in the following manner:'
  header: Authorization
  how_to_obtain: Create an API key in your Lucca account settings.
  location: header
  name: API Key
  type: apiKey
slug: lucca-authentication
source_filename: lucca-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.luccasoftware.com/api-reference/legacy/authentication.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.luccasoftware.com/api-reference/legacy/authentication.md\nsources:\n- https://developers.luccasoftware.com/api-reference/legacy/authentication.md\n- https://developers.luccasoftware.com/documentation/using-api/authentication.md\n- https://developers.luccasoftware.com/documentation/using-api/authentication-spec.md\n- https://developers.luccasoftware.com/api-reference/latest/oauth-scopes.md\ndescription: 'Lucca supports two authentication methods: an API key for the Legacy API and OAuth2 client credentials for the current API.'\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Once you have an API key, you must reference it on all requests against the Legacy APIs through the `Authorization` HTTP header in\n    the following manner:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in your Lucca account settings.\ndocs: https://developers.luccasoftware.com/api-reference/legacy/authentication.md\n\
  note: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lucca/refs/heads/main/authentication/lucca-authentication.yml
summary_line: 1 scheme
tags:
- Company
- HR
- SaaS
- Payroll
- Talent Management
---
