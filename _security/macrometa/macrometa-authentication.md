---
api_key_in:
- header
api_specs:
- filename: macrometa-gdn-openapi-original.json
  format: json
  label: Macrometa Global Data Network (GDN) API
  slug: macrometa-global-data-network-gdn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-gdn-openapi-original.json
- filename: macrometa-photoniq-eds-openapi-original.json
  format: json
  label: PhotonIQ Event Delivery Service (EDS) API
  slug: photoniq-event-delivery-service-eds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-eds-openapi-original.json
- filename: macrometa-photoniq-est-openapi-original.json
  format: json
  label: PhotonIQ Edge Side Tagging (EST) API
  slug: photoniq-edge-side-tagging-est-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-est-openapi-original.json
- filename: macrometa-photoniq-faas-openapi-original.json
  format: json
  label: PhotonIQ Function as a Service (FaaS) API
  slug: photoniq-function-as-a-service-faas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-faas-openapi-original.json
- filename: macrometa-photoniq-fps-openapi-original.json
  format: json
  label: PhotonIQ Fingerprint (FPS) API
  slug: photoniq-fingerprint-fps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-fps-openapi-original.json
- filename: macrometa-photoniq-hss-openapi-original.json
  format: json
  label: PhotonIQ HyperSearch (HSS) API
  slug: photoniq-hypersearch-hss-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-hss-openapi-original.json
- filename: macrometa-photoniq-prerender-openapi-original.json
  format: json
  label: PhotonIQ Prerender Service API
  slug: photoniq-prerender-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-prerender-openapi-original.json
- filename: macrometa-photoniq-vwrs-openapi-original.json
  format: json
  label: PhotonIQ Virtual Waiting Rooms (VWRS) API
  slug: photoniq-virtual-waiting-rooms-vwrs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/openapi/macrometa-photoniq-vwrs-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Macrometa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Macrometa secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Macrometa
provider_slug: macrometa
scheme_count: 2
schemes:
- description: 'Provide an API Key to the `Authorization` header, prefixed with "apikey".


    Example: `Authorization: apikey <key>`'
  in: header
  name: ApiKeyAuth
  parameter: Authorization
  sources:
  - openapi/macrometa-gdn-openapi-original.json
  - openapi/macrometa-photoniq-eds-openapi-original.json
  - openapi/macrometa-photoniq-faas-openapi-original.json
  - openapi/macrometa-photoniq-fps-openapi-original.json
  - openapi/macrometa-photoniq-hss-openapi-original.json
  - openapi/macrometa-photoniq-vwrs-openapi-original.json
  type: apiKey
- bearerFormat: JWT
  description: 'Provide a JSON Web Token (JWT) to the `Authorization` header, prefixed with "bearer".


    Example: `Authorization: bearer <jwt>`'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/macrometa-gdn-openapi-original.json
  type: http
slug: macrometa-authentication
source_filename: macrometa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/macrometa-gdn-openapi-original.json, openapi/macrometa-photoniq-eds-openapi-original.json,\n  openapi/macrometa-photoniq-faas-openapi-original.json, openapi/macrometa-photoniq-fps-openapi-original.json,\n  openapi/macrometa-photoniq-hss-openapi-original.json, openapi/macrometa-photoniq-vwrs-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: |-\n    Provide an API Key to the `Authorization` header, prefixed with \"apikey\".\n\n    Example: `Authorization: apikey <key>`\n  sources:\n  - openapi/macrometa-gdn-openapi-original.json\n  - openapi/macrometa-photoniq-eds-openapi-original.json\n  - openapi/macrometa-photoniq-faas-openapi-original.json\n  - openapi/macrometa-photoniq-fps-openapi-original.json\n  - openapi/macrometa-photoniq-hss-openapi-original.json\n  - openapi/macrometa-photoniq-vwrs-openapi-original.json\n\
  - name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    Provide a JSON Web Token (JWT) to the `Authorization` header, prefixed with \"bearer\".\n\n    Example: `Authorization: bearer <jwt>`\n  sources:\n  - openapi/macrometa-gdn-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/macrometa/refs/heads/main/authentication/macrometa-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Infrastructure
- Edge Computing
- Database
- NoSQL
- Serverless
- Streaming
- Stream Processing
- Real Time
- Web Performance
- CDN
- Search
- Artificial Intelligence
- API
---
