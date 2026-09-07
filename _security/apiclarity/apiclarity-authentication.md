---
anonymous_access: false
api_key_in: []
api_specs:
- filename: apiclarity-api-events-api-openapi.yml
  format: yaml
  label: APIClarity API Events API
  slug: apiclarity-api-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-api-events-api-openapi.yml
- filename: apiclarity-api-inventory-api-openapi.yml
  format: yaml
  label: APIClarity API Inventory API
  slug: apiclarity-api-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-api-inventory-api-openapi.yml
- filename: apiclarity-control-api-openapi.yml
  format: yaml
  label: APIClarity Control API
  slug: apiclarity-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-control-api-openapi.yml
- filename: apiclarity-features-api-openapi.yml
  format: yaml
  label: APIClarity Features API
  slug: apiclarity-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-features-api-openapi.yml
- filename: apiclarity-bfla-module-openapi.yml
  format: yaml
  label: APIClarity BFLA Module API
  slug: apiclarity-bfla-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-bfla-module-openapi.yml
- filename: apiclarity-fuzzer-module-openapi.yml
  format: yaml
  label: APIClarity Fuzzer Module API
  slug: apiclarity-fuzzer-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-fuzzer-module-openapi.yml
- filename: apiclarity-trace-analyzer-module-openapi.yml
  format: yaml
  label: APIClarity Trace Analyzer Module API
  slug: apiclarity-trace-analyzer-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-trace-analyzer-module-openapi.yml
- filename: apiclarity-spec-differ-module-openapi.yml
  format: yaml
  label: APIClarity Spec Differ Module API
  slug: apiclarity-spec-differ-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-spec-differ-module-openapi.yml
- filename: apiclarity-spec-reconstructor-module-openapi.yml
  format: yaml
  label: APIClarity Spec Reconstructor Module API
  slug: apiclarity-spec-reconstructor-module-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-spec-reconstructor-module-openapi.yml
- filename: apiclarity-plugins-telemetry-swagger.yml
  format: yaml
  label: APIClarity Plugins Telemetry API
  slug: apiclarity-plugins-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-plugins-telemetry-swagger.yml
- filename: apiclarity-notifications-openapi.yml
  format: yaml
  label: APIClarity Notifications API
  slug: apiclarity-notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/openapi/apiclarity-notifications-openapi.yml
auth_types:
- apiKey
description: Authentication profile for APIClarity, read from the contracts the project actually publishes in its own source repository. APIClarity is Apache-2.0 software the user deploys into their own Kubernetes cluster — there is no vendor-operated API, no vendor account, and no vendor-issued credential. Everything below is a deployment-local credential.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Apiclarity Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIClarity secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: APIClarity
provider_slug: apiclarity
scheme_count: 1
schemes:
- applies_to: openapi/apiclarity-plugins-telemetry-swagger.yml
  description: '"Optional header to authenticate the trace source." Presented by a traffic-source plugin (Istio WASM filter, taper DaemonSet, Kong, Tyk, Kuma, OpenTelemetry collector) on every call to the plugins telemetry API — POST /telemetry, GET /hostsToTrace and POST /control/newDiscoveredAPIs.'
  evidence: 'parameters.TraceSourceTokenHeader (name: X-Trace-Source-Token, in: header, required: false)'
  header: X-Trace-Source-Token
  in: header
  issuance: The token is minted by the operator's own APIClarity deployment when a trace source is registered through POST /control/traceSources; the created TraceSource object carries a `token` string that the external trace source then presents.
  name: X-Trace-Source-Token
  required: false
  source: https://raw.githubusercontent.com/openclarity/apiclarity/master/plugins/api/swagger.yaml
  type: apiKey
slug: apiclarity-authentication
source_filename: apiclarity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://raw.githubusercontent.com/openclarity/apiclarity/master/plugins/api/swagger.yaml\ndocs: https://github.com/openclarity/apiclarity#readme\ndescription: >-\n  Authentication profile for APIClarity, read from the contracts the project actually\n  publishes in its own source repository. APIClarity is Apache-2.0 software the user\n  deploys into their own Kubernetes cluster — there is no vendor-operated API, no vendor\n  account, and no vendor-issued credential. Everything below is a deployment-local\n  credential.\nsummary:\n  types:\n  - apiKey\n  vendor_issued_credentials: false\n  scheme_count: 1\ncorrection:\n  date: '2026-09-04'\n  note: >-\n    A previous round recorded an `http`/`bearer` scheme named BearerAuth with the description\n    \"deployments commonly require a bearer token\". No APIClarity contract declares it —\n    api/swagger.yaml, api3/core/openapi.yaml, api3/global/openapi.gen.yaml and every module\n\
  \    spec declare zero securitySchemes. It had been written into the API Evangelist-derived\n    openapi/ documents and then read back out as if it were the provider's. It has been\n    removed from those documents and from this profile.\nschemes:\n- name: X-Trace-Source-Token\n  type: apiKey\n  in: header\n  header: X-Trace-Source-Token\n  required: false\n  applies_to: openapi/apiclarity-plugins-telemetry-swagger.yml\n  description: >-\n    \"Optional header to authenticate the trace source.\" Presented by a traffic-source plugin\n    (Istio WASM filter, taper DaemonSet, Kong, Tyk, Kuma, OpenTelemetry collector) on every\n    call to the plugins telemetry API — POST /telemetry, GET /hostsToTrace and\n    POST /control/newDiscoveredAPIs.\n  issuance: >-\n    The token is minted by the operator's own APIClarity deployment when a trace source is\n    registered through POST /control/traceSources; the created TraceSource object carries a\n    `token` string that the external trace source\
  \ then presents.\n  source: https://raw.githubusercontent.com/openclarity/apiclarity/master/plugins/api/swagger.yaml\n  evidence: 'parameters.TraceSourceTokenHeader (name: X-Trace-Source-Token, in: header, required: false)'\nmanagement_api:\n  declared_scheme: none\n  note: >-\n    The APIClarity core/management API (/api, and /api/modules/* for the BFLA, fuzzer,\n    spec-differ, spec-reconstructor and trace-analyzer modules) declares NO securityScheme in\n    any published contract. In the shipped Helm chart the service is cluster-internal and the\n    documented access path is `kubectl port-forward`; the chart exposes server TLS\n    (apiclarity.tls.tlsServerCertsSecretName) but no authentication layer. Any authentication\n    in front of it is the operator's ingress, not something APIClarity publishes.\n  evidence:\n  - https://raw.githubusercontent.com/openclarity/apiclarity/master/api3/global/openapi.gen.yaml\n  - https://raw.githubusercontent.com/openclarity/apiclarity/master/charts/apiclarity/values.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiclarity/refs/heads/main/authentication/apiclarity-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- API Observability
- API Security
- API Traffic Analysis
- Cisco
- Kubernetes
- Open-Source
- OpenAPI Reconstruction
- OpenClarity
- Service Mesh
- Shadow APIs
---
