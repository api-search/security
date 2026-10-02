---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jobspipe-account-api-openapi.yml
  format: yaml
  label: JobsPipe Account API
  slug: jobspipe-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-account-api-openapi.yml
- filename: jobspipe-billing-api-openapi.yml
  format: yaml
  label: JobsPipe Billing API
  slug: jobspipe-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-billing-api-openapi.yml
- filename: jobspipe-companies-api-openapi.yml
  format: yaml
  label: JobsPipe Companies API
  slug: jobspipe-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-companies-api-openapi.yml
- filename: jobspipe-jobs-api-openapi.yml
  format: yaml
  label: JobsPipe Jobs API
  slug: jobspipe-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-jobs-api-openapi.yml
- filename: jobspipe-jobspipe-api-api-openapi.yml
  format: yaml
  label: JobsPipe JobsPipe API
  slug: jobspipe-jobspipe-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-jobspipe-api-api-openapi.yml
- filename: jobspipe-labour-market-insights-api-openapi.yml
  format: yaml
  label: JobsPipe Labour Market Insights API
  slug: jobspipe-labour-market-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-labour-market-insights-api-openapi.yml
- filename: jobspipe-monitors-api-openapi.yml
  format: yaml
  label: JobsPipe Monitors API
  slug: jobspipe-monitors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-monitors-api-openapi.yml
- filename: jobspipe-sandbox-api-openapi.yml
  format: yaml
  label: JobsPipe Sandbox API
  slug: jobspipe-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-sandbox-api-openapi.yml
- filename: jobspipe-stack-api-openapi.yml
  format: yaml
  label: JobsPipe Stack API
  slug: jobspipe-stack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-stack-api-openapi.yml
- filename: jobspipe-technologies-api-openapi.yml
  format: yaml
  label: JobsPipe Technologies API
  slug: jobspipe-technologies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/openapi/jobspipe-technologies-api-openapi.yml
auth_types: []
description: JobsPipe authenticates every API request with a secret Bearer key.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Jobspipe Authentication
name_suffix: Authentication
oauth_flows: []
overview: JobsPipe declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: JobsPipe
provider_slug: jobspipe
scheme_count: 2
schemes:
- evidence: JobsPipe authenticates every API request with a secret Bearer key.
  header: Authorization
  how_to_obtain: Generate an API key in the dashboard (Settings → API Keys). The key starts with jp_live_ and is shown only once. Use it as a Bearer token.
  location: header
  name: Authorization
  type: http-bearer
- evidence: JobsPipe authenticates every API request with a secret Bearer key.
  header: x-api-key
  how_to_obtain: Generate an API key in the dashboard (Settings → API Keys). The key starts with jp_live_ and is shown only once. Send the key in the x-api-key header.
  location: header
  name: x-api-key
  type: apiKey
slug: jobspipe-authentication
source_filename: jobspipe-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.jobspipe.dev/authentication
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.jobspipe.dev/authentication\nsources:\n- https://docs.jobspipe.dev/authentication\n- https://docs.jobspipe.dev/dashboard/api-keys\n- https://docs.jobspipe.dev/quickstart\ndescription: JobsPipe authenticates every API request with a secret Bearer key.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: JobsPipe authenticates every API request with a secret Bearer key.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key in the dashboard (Settings → API Keys). The key starts with jp_live_ and is shown only once. Use it as a\n    Bearer token.\n- type: apiKey\n  name: x-api-key\n  evidence: JobsPipe authenticates every API request with a secret Bearer key.\n  location: header\n  header: x-api-key\n  how_to_obtain: Generate an API key in the dashboard (Settings → API Keys). The key starts with jp_live_ and is shown only once.\
  \ Send the key\n    in the x-api-key header.\nnote: The sandbox endpoints under /v1/sandbox do not require an API key.\ndocs: https://docs.jobspipe.dev/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jobspipe/refs/heads/main/authentication/jobspipe-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Jobs
- API
- Data
- Hiring
---
