---
api_key_in: []
api_specs:
- filename: hotel-engine-catalogservice-api-openapi.yml
  format: yaml
  label: Engine Catalog Service API
  slug: hotel-engine-catalogservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/openapi/hotel-engine-catalogservice-api-openapi.yml
- filename: hotel-engine-contentservice-api-openapi.yml
  format: yaml
  label: Engine Content Service API
  slug: hotel-engine-contentservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/openapi/hotel-engine-contentservice-api-openapi.yml
- filename: hotel-engine-lodgingbookingservice-api-openapi.yml
  format: yaml
  label: Engine Lodging Booking Service API
  slug: hotel-engine-lodgingbookingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/openapi/hotel-engine-lodgingbookingservice-api-openapi.yml
- filename: hotel-engine-lodgingshoppingservice-api-openapi.yml
  format: yaml
  label: Engine Lodging Shopping Service API
  slug: hotel-engine-lodgingshoppingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/openapi/hotel-engine-lodgingshoppingservice-api-openapi.yml
auth_types:
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Hotel Engine Authentication
name_suffix: Authentication
oauth_flows: []
overview: Engine secures its APIs with mutualTLS across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Engine
provider_slug: hotel-engine
scheme_count: 1
schemes:
- credential_request: omni-partnerships@engine.com
  description: Mutual TLS client-certificate authentication. Engine provisions a private key and certificate per partner during onboarding; contact the Omni team to have one issued.
  endpoint: partner-api.engine.com:443
  example_grpc: "grpcurl -protoset descriptor_set.desc \\\n  -key /path/to/private.key \\\n  -cert /path/to/cert.pem \\\n  partner-api.engine.com:443 \\\n  engine.content.api.v1.ContentService.ListProperties\n"
  name: mTLS
  provisioning: manual, via the Omni partnership process
  sources:
  - https://engine-public.github.io/engine-partner-api/integration-guide.html
  - live TLS probe of partner-api.engine.com:443 (2026-08-04)
  transport:
  - grpc
  - http-json
  type: mutualTLS
slug: hotel-engine-authentication
source_filename: hotel-engine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: https://engine-public.github.io/engine-partner-api/integration-guide.html\ndocs: https://engine-public.github.io/engine-partner-api/integration-guide.html\nsummary:\n  types: [mutualTLS]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The Omni Partner API authenticates exclusively with Mutual TLS (mTLS) client certificates —\n    on both the gRPC and the HTTP/JSON surface. There are no API keys, no bearer tokens, and no\n    OAuth. Because mTLS is a transport-layer mechanism, it is not expressible in Swagger 2.0\n    securityDefinitions, so the published spec carries no securityDefinitions block at all; the\n    auth contract lives only in the prose docs. This was verified live: a TLS 1.3 handshake to\n    partner-api.engine.com:443 emits a \"Request CERT\" (certificate request) message and the\n    connection yields no HTTP response without a client certificate.\nschemes:\n  - name: mTLS\n    type: mutualTLS\n    transport:\
  \ [grpc, http-json]\n    endpoint: partner-api.engine.com:443\n    description: >-\n      Mutual TLS client-certificate authentication. Engine provisions a private key and\n      certificate per partner during onboarding; contact the Omni team to have one issued.\n    provisioning: manual, via the Omni partnership process\n    credential_request: omni-partnerships@engine.com\n    sources:\n      - https://engine-public.github.io/engine-partner-api/integration-guide.html\n      - live TLS probe of partner-api.engine.com:443 (2026-08-04)\n    example_grpc: |\n      grpcurl -protoset descriptor_set.desc \\\n        -key /path/to/private.key \\\n        -cert /path/to/cert.pem \\\n        partner-api.engine.com:443 \\\n        engine.content.api.v1.ContentService.ListProperties\nspec_gap:\n  finding: >-\n    openapi/_original/hotel-engine-omni-partner-api-2.4.0-swagger-original.json declares no\n    securityDefinitions and no security requirement on any of its 11 operations, so an agent or\n\
  \    codegen tool reading the spec alone cannot discover that a client certificate is required.\n  recommendation: >-\n    Emit a Swagger `securityDefinitions` stub or migrate the generated document to OpenAPI 3.1,\n    where `type: mutualTLS` is a first-class security scheme. Engine already maintains its own\n    protoc-gen-openapi plugin that produces OpenAPI 3.1, so the path exists in-house.\nonboarding:\n  self_serve: false\n  process: >-\n    Partnership agreement required. Complete the intake form at https://omni.engine.com/#contact\n    and contact omni-partnerships@engine.com; a sandbox environment is provisioned on approval.\nrelated:\n  conventions: conventions/hotel-engine-conventions.yml\n  domain_security: security/hotel-engine-domain-security.yml\n  scopes: null   # no OAuth surface — scopes/ intentionally not emitted\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hotel-engine/refs/heads/main/authentication/hotel-engine-authentication.yml
summary_line: mutualTLS · 1 scheme
tags:
- Company
- Travel
- Business Travel
- Lodging
- Hotels
- Booking
- Travel Management
- Expense Management
- Payments
- gRPC
- Protobuf
- Partner API
---
