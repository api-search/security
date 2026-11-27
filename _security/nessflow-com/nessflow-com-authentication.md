---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nessflow-com-account-api-openapi.yml
  format: yaml
  label: NessFlow Account API
  slug: nessflow-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nessflow-com/openapi/nessflow-com-account-api-openapi.yml
- filename: nessflow-com-campaigns-api-openapi.yml
  format: yaml
  label: NessFlow Campaigns API
  slug: nessflow-com-campaigns-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nessflow-com/openapi/nessflow-com-campaigns-api-openapi.yml
- filename: nessflow-com-crawls-api-openapi.yml
  format: yaml
  label: NessFlow Crawls API
  slug: nessflow-com-crawls-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nessflow-com/openapi/nessflow-com-crawls-api-openapi.yml
- filename: nessflow-com-exports-api-openapi.yml
  format: yaml
  label: NessFlow Exports API
  slug: nessflow-com-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nessflow-com/openapi/nessflow-com-exports-api-openapi.yml
- filename: nessflow-com-modules-api-openapi.yml
  format: yaml
  label: NessFlow Modules API
  slug: nessflow-com-modules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nessflow-com/openapi/nessflow-com-modules-api-openapi.yml
- filename: nessflow-com-projects-api-openapi.yml
  format: yaml
  label: NessFlow Projects API
  slug: nessflow-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nessflow-com/openapi/nessflow-com-projects-api-openapi.yml
- filename: nessflow-com-recommendations-api-openapi.yml
  format: yaml
  label: NessFlow Recommendations API
  slug: nessflow-com-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nessflow-com/openapi/nessflow-com-recommendations-api-openapi.yml
- filename: nessflow-com-webhooks-api-openapi.yml
  format: yaml
  label: NessFlow Webhooks API
  slug: nessflow-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nessflow-com/openapi/nessflow-com-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes for NessFlow API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: NessFlow Authentication
name_suffix: Authentication
oauth_flows: []
overview: NessFlow declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: NessFlow
provider_slug: nessflow-com
scheme_count: 1
schemes:
- evidence: 'Every request carries the token in the Authorization header, as Bearer followed by the token:'
  header: Authorization
  how_to_obtain: Open your team's API screen, in the team settings, then Create a token.
  location: header
  name: Bearer token
  type: http-bearer
slug: nessflow-com-authentication
source_filename: nessflow-com-authentication.yml
source_heading: Authentication Profile
source_url: https://nessflow.com/en/developers/authentication
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nessflow.com/en/developers/authentication\nsources:\n- https://nessflow.com/en/developers/authentication\n- https://nessflow.com/en/developers/quickstart\n- https://nessflow.com/en/developers/reference/account\n- https://nessflow.com/en/developers/quickstart.md\ndescription: Authentication schemes for NessFlow API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Every request carries the token in the Authorization header, as Bearer followed by the token:'\n  location: header\n  header: Authorization\n  how_to_obtain: Open your team's API screen, in the team settings, then Create a token.\nnote: No OAuth2, apiKey, or other authentication methods are documented.\ndocs: https://nessflow.com/en/developers/authentication\n"
source_yaml_url: https://artifacts.apis.io/nessflow-com/authentication/nessflow-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- SEO
- Artificial Intelligence
- Analytics
- Visibility
---
