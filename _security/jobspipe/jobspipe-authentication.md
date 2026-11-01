---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jobspipe-account-api-openapi.yml
  format: yaml
  label: JobsPipe Account API
  slug: jobspipe-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobspipe/openapi/jobspipe-account-api-openapi.yml
- filename: jobspipe-billing-api-openapi.yml
  format: yaml
  label: JobsPipe Billing API
  slug: jobspipe-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobspipe/openapi/jobspipe-billing-api-openapi.yml
- filename: jobspipe-companies-api-openapi.yml
  format: yaml
  label: JobsPipe Companies API
  slug: jobspipe-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobspipe/openapi/jobspipe-companies-api-openapi.yml
- filename: jobspipe-jobs-api-openapi.yml
  format: yaml
  label: JobsPipe Jobs API
  slug: jobspipe-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobspipe/openapi/jobspipe-jobs-api-openapi.yml
- filename: jobspipe-jobspipe-api-api-openapi.yml
  format: yaml
  label: JobsPipe JobsPipe API
  slug: jobspipe-jobspipe-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobspipe/openapi/jobspipe-jobspipe-api-api-openapi.yml
- filename: jobspipe-labour-market-insights-api-openapi.yml
  format: yaml
  label: JobsPipe Labour Market Insights API
  slug: jobspipe-labour-market-insights-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobspipe/openapi/jobspipe-labour-market-insights-api-openapi.yml
- filename: jobspipe-monitors-api-openapi.yml
  format: yaml
  label: JobsPipe Monitors API
  slug: jobspipe-monitors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobspipe/openapi/jobspipe-monitors-api-openapi.yml
- filename: jobspipe-sandbox-api-openapi.yml
  format: yaml
  label: JobsPipe Sandbox API
  slug: jobspipe-sandbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobspipe/openapi/jobspipe-sandbox-api-openapi.yml
- filename: jobspipe-stack-api-openapi.yml
  format: yaml
  label: JobsPipe Stack API
  slug: jobspipe-stack-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobspipe/openapi/jobspipe-stack-api-openapi.yml
- filename: jobspipe-technologies-api-openapi.yml
  format: yaml
  label: JobsPipe Technologies API
  slug: jobspipe-technologies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobspipe/openapi/jobspipe-technologies-api-openapi.yml
- filename: jobspipe-contacts-api-openapi.yml
  format: yaml
  label: JobsPipe Contacts API
  slug: jobspipe-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobspipe/openapi/jobspipe-contacts-api-openapi.yml
- filename: jobspipe-layoffs-api-openapi.yml
  format: yaml
  label: JobsPipe Layoffs API
  slug: jobspipe-layoffs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobspipe/openapi/jobspipe-layoffs-api-openapi.yml
- filename: jobspipe-live-api-openapi.yml
  format: yaml
  label: JobsPipe Live API
  slug: jobspipe-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jobspipe/openapi/jobspipe-live-api-openapi.yml
auth_types: []
description: JobsPipe uses API keys that are sent as Bearer tokens or as a custom header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Jobspipe Authentication
name_suffix: Authentication
oauth_flows: []
overview: JobsPipe declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: JobsPipe
provider_slug: jobspipe
scheme_count: 1
schemes:
- evidence: JobsPipe authenticates every API request with a secret Bearer key.
  header: Authorization
  how_to_obtain: Generate API key in the dashboard (Settings → API Keys). The key starts with jp_live_ and is shown only once.
  location: header
  name: Bearer
  type: http-bearer
slug: jobspipe-authentication
source_filename: jobspipe-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.jobspipe.dev/authentication
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.jobspipe.dev/authentication\nsources:\n- https://docs.jobspipe.dev/authentication\n- https://docs.jobspipe.dev/dashboard/api-keys\n- https://docs.jobspipe.dev/quickstart\ndescription: JobsPipe uses API keys that are sent as Bearer tokens or as a custom header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: JobsPipe authenticates every API request with a secret Bearer key.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate API key in the dashboard (Settings → API Keys). The key starts with jp_live_ and is shown only once.\ndocs: https://docs.jobspipe.dev/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/jobspipe/authentication/jobspipe-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Job
- Data
- Hiring
- JobsAPI
---
