---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Buoyant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Buoyant declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Buoyant
provider_slug: buoyant
scheme_count: 2
schemes:
- contract: grpc/buoyant-linkerd-proxy-api-identity.proto
  credentials:
  - name: Kubernetes ServiceAccount projected token
    transport: gRPC request field
  description: Every meshed workload obtains a short-lived mTLS leaf certificate by calling the Identity service's Certify RPC with its Kubernetes ServiceAccount token. Identity is bound to the ServiceAccount, not to the pod IP or hostname, which is what makes Linkerd's AuthorizationPolicy checks identity-based rather than network-based.
  id: linkerd-workload-identity
  rotation: Leaf certificates are short-lived and auto-rotated. Trust anchor rotation was manual until Buoyant Enterprise for Linkerd 2.20.0 introduced an operator that automates it.
  surface: In-cluster Linkerd control plane (io.linkerd.proxy.identity.Identity)
  type: mutualTLS
- credentials:
  - location: Helm value
    name: api.clientID
  - location: Helm value
    name: api.clientSecret
  - location: data field of the Kubernetes secret buoyant-cloud-org-credentials
    name: client_id
  - location: data field of the Kubernetes secret buoyant-cloud-org-credentials
    name: client_secret
  description: The Buoyant Cloud agent authenticates to Buoyant Cloud with an org-scoped client ID and secret issued in the Buoyant Cloud workspace. These are supplied either as Helm values or as a pre-created Kubernetes secret. This is a machine-to-machine credential for the agent, not a public developer API key programme — Buoyant publishes no developer API key issuance flow.
  id: buoyant-cloud-agent-credentials
  issuance: https://buoyant.cloud/settings
  surface: api.buoyant.cloud (Buoyant Cloud agent telemetry + configuration)
  transport: 'gRPC over HTTPS to api.buoyant.cloud. Probed 2026-09-04: any non-gRPC request returns HTTP 415 with content-type application/grpc, grpc-status 3, grpc-message "invalid gRPC request content-type". HSTS is enforced (max-age=31536000; includeSubDomains).'
  type: clientCredentials
slug: buoyant-authentication
source_filename: buoyant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Buoyant\nproviderId: buoyant\ngenerated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://docs.buoyant.io/buoyant-cloud/tasks/programmatic-agent-install/,\n  https://docs.buoyant.io/buoyant-cloud/tasks/routing-requests-through-internet-proxy/,\n  grpc/buoyant-linkerd-proxy-api-identity.proto (saved verbatim in this repo), and a\n  live probe of https://api.buoyant.cloud (2026-09-04).\nnote: >-\n  There is no OpenAPI to derive from — Buoyant's machine-readable contracts are\n  protobuf. Two distinct authentication surfaces exist and they are not\n  interchangeable: an in-cluster mTLS identity plane, and a client-credentials\n  handshake between the Buoyant Cloud agent and api.buoyant.cloud.\nschemes:\n  - id: linkerd-workload-identity\n    surface: In-cluster Linkerd control plane (io.linkerd.proxy.identity.Identity)\n    type: mutualTLS\n    description: >-\n      Every meshed workload obtains\
  \ a short-lived mTLS leaf certificate by calling the\n      Identity service's Certify RPC with its Kubernetes ServiceAccount token. Identity\n      is bound to the ServiceAccount, not to the pod IP or hostname, which is what makes\n      Linkerd's AuthorizationPolicy checks identity-based rather than network-based.\n    contract: grpc/buoyant-linkerd-proxy-api-identity.proto\n    credentials:\n      - name: Kubernetes ServiceAccount projected token\n        transport: gRPC request field\n    rotation: >-\n      Leaf certificates are short-lived and auto-rotated. Trust anchor rotation was\n      manual until Buoyant Enterprise for Linkerd 2.20.0 introduced an operator that\n      automates it.\n  - id: buoyant-cloud-agent-credentials\n    surface: api.buoyant.cloud (Buoyant Cloud agent telemetry + configuration)\n    type: clientCredentials\n    description: >-\n      The Buoyant Cloud agent authenticates to Buoyant Cloud with an org-scoped client\n      ID and secret issued in the Buoyant\
  \ Cloud workspace. These are supplied either as\n      Helm values or as a pre-created Kubernetes secret. This is a machine-to-machine\n      credential for the agent, not a public developer API key programme — Buoyant\n      publishes no developer API key issuance flow.\n    credentials:\n      - name: api.clientID\n        location: Helm value\n      - name: api.clientSecret\n        location: Helm value\n      - name: client_id\n        location: data field of the Kubernetes secret buoyant-cloud-org-credentials\n      - name: client_secret\n        location: data field of the Kubernetes secret buoyant-cloud-org-credentials\n    issuance: https://buoyant.cloud/settings\n    transport: >-\n      gRPC over HTTPS to api.buoyant.cloud. Probed 2026-09-04: any non-gRPC request\n      returns HTTP 415 with content-type application/grpc, grpc-status 3,\n      grpc-message \"invalid gRPC request content-type\". HSTS is enforced\n      (max-age=31536000; includeSubDomains).\noauth2:\n  published:\
  \ false\n  note: >-\n    No OAuth 2.0 or OpenID Connect discovery document is served on any Buoyant or\n    Linkerd host — see well-known/buoyant-well-known.yml. Buoyant Cloud user sign-in is\n    a first-party web login at buoyant.cloud, not a documented delegated-authorization\n    flow for third-party clients.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/buoyant/refs/heads/main/authentication/buoyant-authentication.yml
summary_line: 2 schemes
tags:
- AI Observability
- Kubernetes
- Linkerd
- mTLS
- Observability
- Service Mesh
- Zero Trust
---
