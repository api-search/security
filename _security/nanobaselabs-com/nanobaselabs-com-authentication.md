---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: nanobaselabs-com-account-api-openapi.yml
  format: yaml
  label: NanoBase™ Account API
  slug: nanobaselabs-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanobaselabs-com/openapi/nanobaselabs-com-account-api-openapi.yml
- filename: nanobaselabs-com-ai-api-openapi.yml
  format: yaml
  label: NanoBase™ AI API
  slug: nanobaselabs-com-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanobaselabs-com/openapi/nanobaselabs-com-ai-api-openapi.yml
- filename: nanobaselabs-com-changelog-api-openapi.yml
  format: yaml
  label: NanoBase™ Changelog API
  slug: nanobaselabs-com-changelog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanobaselabs-com/openapi/nanobaselabs-com-changelog-api-openapi.yml
- filename: nanobaselabs-com-check-api-openapi.yml
  format: yaml
  label: NanoBase™ Check API
  slug: nanobaselabs-com-check-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanobaselabs-com/openapi/nanobaselabs-com-check-api-openapi.yml
- filename: nanobaselabs-com-inci-api-openapi.yml
  format: yaml
  label: NanoBase™ Inci API
  slug: nanobaselabs-com-inci-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanobaselabs-com/openapi/nanobaselabs-com-inci-api-openapi.yml
- filename: nanobaselabs-com-ingredients-api-openapi.yml
  format: yaml
  label: NanoBase™ Ingredients API
  slug: nanobaselabs-com-ingredients-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanobaselabs-com/openapi/nanobaselabs-com-ingredients-api-openapi.yml
- filename: nanobaselabs-com-lib-api-openapi.yml
  format: yaml
  label: NanoBase™ Lib API
  slug: nanobaselabs-com-lib-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanobaselabs-com/openapi/nanobaselabs-com-lib-api-openapi.yml
- filename: nanobaselabs-com-terms-api-openapi.yml
  format: yaml
  label: NanoBase™ Terms API
  slug: nanobaselabs-com-terms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanobaselabs-com/openapi/nanobaselabs-com-terms-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: NanoBase™ Authentication
name_suffix: Authentication
oauth_flows: []
overview: NanoBase™ secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: NanoBase™
provider_slug: nanobaselabs-com
scheme_count: 1
schemes:
- in: header
  name: key
  parameter: x-nb-key
  sources:
  - openapi/nanobaselabs-com-openapi.json
  type: apiKey
slug: nanobaselabs-com-authentication
source_filename: nanobaselabs-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nanobaselabs-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: key\n  type: apiKey\n  in: header\n  parameter: x-nb-key\n  sources:\n  - openapi/nanobaselabs-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nanobaselabs-com/authentication/nanobaselabs-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cosmetics
- Nanoscience
- Research
- Manufacturing
- Beauty
---
