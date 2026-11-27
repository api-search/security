---
anonymous_access: false
api_key_in: []
api_specs:
- filename: esignsimple-com-account-api-openapi.yml
  format: yaml
  label: eSignSimple Account API
  slug: esignsimple-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esignsimple-com/openapi/esignsimple-com-account-api-openapi.yml
- filename: esignsimple-com-documents-api-openapi.yml
  format: yaml
  label: eSignSimple Documents API
  slug: esignsimple-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esignsimple-com/openapi/esignsimple-com-documents-api-openapi.yml
- filename: esignsimple-com-templates-api-openapi.yml
  format: yaml
  label: eSignSimple Templates API
  slug: esignsimple-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esignsimple-com/openapi/esignsimple-com-templates-api-openapi.yml
- filename: esignsimple-com-verification-api-openapi.yml
  format: yaml
  label: eSignSimple Verification API
  slug: esignsimple-com-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/esignsimple-com/openapi/esignsimple-com-verification-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: eSignSimple Authentication
name_suffix: Authentication
oauth_flows: []
overview: eSignSimple secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: eSignSimple
provider_slug: esignsimple-com
scheme_count: 1
schemes:
- description: API key `es_live_…` from Settings → Developers.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/esignsimple-com-openapi.yml
  type: http
slug: esignsimple-com-authentication
source_filename: esignsimple-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/esignsimple-com-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key `es_live_…` from Settings → Developers.\n  sources:\n  - openapi/esignsimple-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/esignsimple-com/authentication/esignsimple-com-authentication.yml
summary_line: http · 1 scheme
tags:
- E-Signature
- Templates
- Bulk Sending
- Web Forms
- ID Verification
---
