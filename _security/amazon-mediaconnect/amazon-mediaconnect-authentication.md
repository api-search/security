---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: amazon-mediaconnect-bridges-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Bridges API
  slug: amazon-mediaconnect-bridges-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-bridges-api-openapi.yml
- filename: amazon-mediaconnect-entitlements-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Entitlements API
  slug: amazon-mediaconnect-entitlements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-entitlements-api-openapi.yml
- filename: amazon-mediaconnect-flows-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Flows API
  slug: amazon-mediaconnect-flows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-flows-api-openapi.yml
- filename: amazon-mediaconnect-gateway-instances-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Gateway Instances API
  slug: amazon-mediaconnect-gateway-instances-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-gateway-instances-api-openapi.yml
- filename: amazon-mediaconnect-gateways-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Gateways API
  slug: amazon-mediaconnect-gateways-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-gateways-api-openapi.yml
- filename: amazon-mediaconnect-offerings-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Offerings API
  slug: amazon-mediaconnect-offerings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-offerings-api-openapi.yml
- filename: amazon-mediaconnect-reservations-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Reservations API
  slug: amazon-mediaconnect-reservations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-reservations-api-openapi.yml
- filename: amazon-mediaconnect-tags-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Tags API
  slug: amazon-mediaconnect-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-tags-api-openapi.yml
- filename: amazon-mediaconnect-destinationendpoint-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Mediaconnect Destinationendpoint API
  slug: amazon-mediaconnect-destinationendpoint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-destinationendpoint-api-openapi.yml
- filename: amazon-mediaconnect-mediastreams-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Mediaconnect Mediastreams API
  slug: amazon-mediaconnect-mediastreams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-mediastreams-api-openapi.yml
- filename: amazon-mediaconnect-operations-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Mediaconnect Operations API
  slug: amazon-mediaconnect-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-operations-api-openapi.yml
- filename: amazon-mediaconnect-outputs-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Mediaconnect Outputs API
  slug: amazon-mediaconnect-outputs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-outputs-api-openapi.yml
- filename: amazon-mediaconnect-routerinput-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Mediaconnect Routerinput API
  slug: amazon-mediaconnect-routerinput-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-routerinput-api-openapi.yml
- filename: amazon-mediaconnect-routernetworkinterface-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Mediaconnect Routernetworkinterface API
  slug: amazon-mediaconnect-routernetworkinterface-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-routernetworkinterface-api-openapi.yml
- filename: amazon-mediaconnect-routeroutput-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Mediaconnect Routeroutput API
  slug: amazon-mediaconnect-routeroutput-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-routeroutput-api-openapi.yml
- filename: amazon-mediaconnect-source-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Mediaconnect Source API
  slug: amazon-mediaconnect-source-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-source-api-openapi.yml
- filename: amazon-mediaconnect-sourceendpoint-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Mediaconnect Sourceendpoint API
  slug: amazon-mediaconnect-sourceendpoint-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-sourceendpoint-api-openapi.yml
- filename: amazon-mediaconnect-sources-api-openapi.yml
  format: yaml
  label: Amazon MediaConnect Mediaconnect Sources API
  slug: amazon-mediaconnect-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/amazon-mediaconnect/openapi/amazon-mediaconnect-sources-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Amazon Mediaconnect Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amazon MediaConnect secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amazon MediaConnect
provider_slug: amazon-mediaconnect
scheme_count: 1
schemes:
- description: Amazon Signature authorization v4
  in: header
  name: hmac
  parameter: Authorization
  sources:
  - openapi/amazon-mediaconnect-openapi-original.yml
  type: apiKey
slug: amazon-mediaconnect-authentication
source_filename: amazon-mediaconnect-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amazon-mediaconnect-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: hmac\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Amazon Signature authorization v4\n  sources:\n  - openapi/amazon-mediaconnect-openapi-original.yml\n"
source_yaml_url: https://artifacts.apis.io/amazon-mediaconnect/authentication/amazon-mediaconnect-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Broadcasting
- Live Streaming
- Media
- Media Transport
---
