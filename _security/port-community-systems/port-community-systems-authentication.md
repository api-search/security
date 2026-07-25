---
api_key_in: []
api_specs:
- filename: port-community-systems-cargomanifests-api-openapi.yml
  format: yaml
  label: Port Community Systems CargoManifests API
  slug: port-community-systems-cargomanifests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/openapi/port-community-systems-cargomanifests-api-openapi.yml
- filename: port-community-systems-containers-api-openapi.yml
  format: yaml
  label: Port Community Systems Containers API
  slug: port-community-systems-containers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/openapi/port-community-systems-containers-api-openapi.yml
- filename: port-community-systems-customsdeclarations-api-openapi.yml
  format: yaml
  label: Port Community Systems CustomsDeclarations API
  slug: port-community-systems-customsdeclarations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/openapi/port-community-systems-customsdeclarations-api-openapi.yml
- filename: port-community-systems-hazardouscargo-api-openapi.yml
  format: yaml
  label: Port Community Systems HazardousCargo API
  slug: port-community-systems-hazardouscargo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/openapi/port-community-systems-hazardouscargo-api-openapi.yml
- filename: port-community-systems-vesselcalls-api-openapi.yml
  format: yaml
  label: Port Community Systems VesselCalls API
  slug: port-community-systems-vesselcalls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/openapi/port-community-systems-vesselcalls-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Port Community Systems Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Port Community Systems secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Port Community Systems
provider_slug: port-community-systems
scheme_count: 1
schemes:
- flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://auth.portbase.com/oauth2/token
  name: oauth2
  sources:
  - openapi/portbase-port-community-openapi.yml
  type: oauth2
slug: port-community-systems-authentication
source_filename: port-community-systems-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/portbase-port-community-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.portbase.com/oauth2/token\n    scopes: 4\n  sources:\n  - openapi/portbase-port-community-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/port-community-systems/refs/heads/main/authentication/port-community-systems-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Maritime
- Port
- Logistics
- Customs
- Cargo
- Shipping
---
