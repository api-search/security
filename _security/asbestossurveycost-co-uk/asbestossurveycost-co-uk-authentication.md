---
anonymous_access: false
api_key_in: []
api_specs:
- filename: asbestossurveycost-co-uk-dataset-api-openapi.yml
  format: yaml
  label: Asbestos Survey Cost UK Dataset API
  slug: asbestossurveycost-co-uk-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asbestossurveycost-co-uk/openapi/asbestossurveycost-co-uk-dataset-api-openapi.yml
- filename: asbestossurveycost-co-uk-enquiry-api-openapi.yml
  format: yaml
  label: Asbestos Survey Cost UK Enquiry API
  slug: asbestossurveycost-co-uk-enquiry-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asbestossurveycost-co-uk/openapi/asbestossurveycost-co-uk-enquiry-api-openapi.yml
- filename: asbestossurveycost-co-uk-entities-api-openapi.yml
  format: yaml
  label: Asbestos Survey Cost UK Entities API
  slug: asbestossurveycost-co-uk-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asbestossurveycost-co-uk/openapi/asbestossurveycost-co-uk-entities-api-openapi.yml
- filename: asbestossurveycost-co-uk-mcp-api-openapi.yml
  format: yaml
  label: Asbestos Survey Cost UK MCP API
  slug: asbestossurveycost-co-uk-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/asbestossurveycost-co-uk/openapi/asbestossurveycost-co-uk-mcp-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Asbestossurveycost Co Uk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Asbestos Survey Cost UK secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Asbestos Survey Cost UK
provider_slug: asbestossurveycost-co-uk
scheme_count: 1
schemes:
- description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk entity export requires one.'
  name: accessKey
  scheme: bearer
  sources:
  - openapi/asbestossurveycost-co-uk-openapi.json
  - openapi/asbestossurveycost.co.uk.json
  type: http
slug: asbestossurveycost-co-uk-authentication
source_filename: asbestossurveycost-co-uk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: derived\nsource: openapi/asbestossurveycost-co-uk-openapi.json, openapi/asbestossurveycost.co.uk.json\nsummary:\n  types:\n  - http\nschemes:\n- name: accessKey\n  type: http\n  scheme: bearer\n  description: 'An access key (emk_...): free tier without it, a named budget with it; the bulk\n    entity export requires one.'\n  sources:\n  - openapi/asbestossurveycost-co-uk-openapi.json\n  - openapi/asbestossurveycost.co.uk.json\n"
source_yaml_url: https://artifacts.apis.io/asbestossurveycost-co-uk/authentication/asbestossurveycost-co-uk-authentication.yml
summary_line: http · 1 scheme
tags:
- Asbestos
- Surveys
- United Kingdom
- Contractors
- Licensing
---
