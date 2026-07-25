---
api_key_in:
- header
api_specs:
- filename: amazon-simspace-weaver-createsnapshot-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Createsnapshot API
  slug: amazon-simspace-weaver-createsnapshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-createsnapshot-api-openapi.yml
- filename: amazon-simspace-weaver-deleteapp-app-domain-simulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Deleteapp#app&domain&simulation API
  slug: amazon-simspace-weaver-deleteapp-app-domain-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-deleteapp-app-domain-simulation-api-openapi.yml
- filename: amazon-simspace-weaver-deletesimulation-simulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Deletesimulation#simulation API
  slug: amazon-simspace-weaver-deletesimulation-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-deletesimulation-simulation-api-openapi.yml
- filename: amazon-simspace-weaver-describeapp-app-domain-simulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Describeapp#app&domain&simulation API
  slug: amazon-simspace-weaver-describeapp-app-domain-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-describeapp-app-domain-simulation-api-openapi.yml
- filename: amazon-simspace-weaver-describesimulation-simulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Describesimulation#simulation API
  slug: amazon-simspace-weaver-describesimulation-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-describesimulation-simulation-api-openapi.yml
- filename: amazon-simspace-weaver-listapps-simulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Listapps#simulation API
  slug: amazon-simspace-weaver-listapps-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-listapps-simulation-api-openapi.yml
- filename: amazon-simspace-weaver-listsimulations-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Listsimulations API
  slug: amazon-simspace-weaver-listsimulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-listsimulations-api-openapi.yml
- filename: amazon-simspace-weaver-startapp-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Startapp API
  slug: amazon-simspace-weaver-startapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-startapp-api-openapi.yml
- filename: amazon-simspace-weaver-startclock-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Startclock API
  slug: amazon-simspace-weaver-startclock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-startclock-api-openapi.yml
- filename: amazon-simspace-weaver-startsimulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Startsimulation API
  slug: amazon-simspace-weaver-startsimulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-startsimulation-api-openapi.yml
- filename: amazon-simspace-weaver-stopapp-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Stopapp API
  slug: amazon-simspace-weaver-stopapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-stopapp-api-openapi.yml
- filename: amazon-simspace-weaver-stopclock-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Stopclock API
  slug: amazon-simspace-weaver-stopclock-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-stopclock-api-openapi.yml
- filename: amazon-simspace-weaver-stopsimulation-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Stopsimulation API
  slug: amazon-simspace-weaver-stopsimulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-stopsimulation-api-openapi.yml
- filename: amazon-simspace-weaver-tags-api-openapi.yml
  format: yaml
  label: Amazon SimSpace Weaver Tags API
  slug: amazon-simspace-weaver-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/openapi/amazon-simspace-weaver-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Amazon Simspace Weaver Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon SimSpace Weaver secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon SimSpace Weaver
provider_slug: amazon-simspace-weaver
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-simspace-weaver.yaml
  type: apiKey
slug: amazon-simspace-weaver-authentication
source_filename: amazon-simspace-weaver-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-simspace-weaver.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-simspace-weaver.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amazon-simspace-weaver/refs/heads/main/authentication/amazon-simspace-weaver-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Defense
- Digital Twin
- Simulation
- Spatial Simulation
---
