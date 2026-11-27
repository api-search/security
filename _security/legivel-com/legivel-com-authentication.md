---
anonymous_access: false
api_key_in: []
api_specs:
- filename: legivel-com-health-api-openapi.yml
  format: yaml
  label: legivel Health API
  slug: legivel-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legivel-com/openapi/legivel-com-health-api-openapi.yml
- filename: legivel-com-openapi-json-api-openapi.yml
  format: yaml
  label: legivel Openapi.json API
  slug: legivel-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legivel-com/openapi/legivel-com-openapi-json-api-openapi.yml
- filename: legivel-com-render-api-openapi.yml
  format: yaml
  label: legivel Render API
  slug: legivel-com-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legivel-com/openapi/legivel-com-render-api-openapi.yml
- filename: legivel-com-templates-api-openapi.yml
  format: yaml
  label: legivel Templates API
  slug: legivel-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legivel-com/openapi/legivel-com-templates-api-openapi.yml
- filename: legivel-com-usage-api-openapi.yml
  format: yaml
  label: legivel Usage API
  slug: legivel-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/legivel-com/openapi/legivel-com-usage-api-openapi.yml
auth_types: []
description: Authentication schemes for legivel API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: legivel Authentication
name_suffix: Authentication
oauth_flows: []
overview: legivel declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: legivel
provider_slug: legivel-com
scheme_count: 1
schemes:
- evidence: 'Every request carries a Bearer token: an API key from the account page.'
  header: Authorization
  how_to_obtain: Create an API key on the account page.
  location: header
  name: Bearer
  type: http-bearer
slug: legivel-com-authentication
source_filename: legivel-com-authentication.yml
source_heading: Authentication Profile
source_url: https://legivel.com/docs/api-key.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://legivel.com/docs/api-key.md\nsources:\n- https://legivel.com/docs/api-key.md\n- https://legivel.com/docs/authentication.md\n- https://legivel.com/docs/api-key\n- https://legivel.com/docs/authentication\ndescription: Authentication schemes for legivel API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request carries a Bearer token: an API key from the account page.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key on the account page.\ndocs: https://legivel.com/docs/api-key.md\n"
source_yaml_url: https://artifacts.apis.io/legivel-com/authentication/legivel-com-authentication.yml
summary_line: 1 scheme
tags:
- Markdown
- PDF
- Conversion
- Software-as-a-Service
---
