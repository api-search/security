---
anonymous_access: false
api_key_in: []
api_specs:
- filename: quady3d-com-account-api-openapi.yml
  format: yaml
  label: Quady3D AI Account API
  slug: quady3d-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-account-api-openapi.yml
- filename: quady3d-com-assets-api-openapi.yml
  format: yaml
  label: Quady3D AI Assets API
  slug: quady3d-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-assets-api-openapi.yml
- filename: quady3d-com-jobs-api-openapi.yml
  format: yaml
  label: Quady3D AI Jobs API
  slug: quady3d-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-jobs-api-openapi.yml
- filename: quady3d-com-models-api-openapi.yml
  format: yaml
  label: Quady3D AI Models API
  slug: quady3d-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-models-api-openapi.yml
- filename: quady3d-com-quotes-api-openapi.yml
  format: yaml
  label: Quady3D AI Quotes API
  slug: quady3d-com-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-quotes-api-openapi.yml
- filename: quady3d-com-uploads-api-openapi.yml
  format: yaml
  label: Quady3D AI Uploads API
  slug: quady3d-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-uploads-api-openapi.yml
- filename: quady3d-com-open-api-api-openapi.yml
  format: yaml
  label: Quady3D AI Open API
  slug: quady3d-com-open-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-open-api-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Quady3D AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quady3D AI secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Quady3D AI
provider_slug: quady3d-com
scheme_count: 1
schemes:
- description: Use a dedicated verified-account Key. Never put the Key in a URL, browser bundle or shared project.
  name: Quady3DKey
  scheme: bearer
  sources:
  - openapi/quady3d-com-openapi.json
  type: http
slug: quady3d-com-authentication
source_filename: quady3d-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/quady3d-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: Quady3DKey\n  type: http\n  scheme: bearer\n  description: Use a dedicated verified-account Key. Never put the Key in a URL, browser bundle\n    or shared project.\n  sources:\n  - openapi/quady3d-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/quady3d-com/authentication/quady3d-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- 3D
- Generation
- Image
- Text
---
