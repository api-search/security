---
api_key_in: []
auth_types: []
description: 'Authentication profile for Ambient Mesh. Derived from documentation, not from an OpenAPI securitySchemes block — no OpenAPI exists for this provider (see x-coverage in apis.yml). Two distinct planes have to be kept apart here, and conflating them is the easy mistake: the CONFIGURATION plane is the operator''s own Kubernetes API server, and the DATA plane is workload-to-workload mTLS that Ambient Mesh itself provides.'
kind: authentication
layout: security
method: searched
name: Ambient Mesh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ambient Mesh declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Ambient Mesh
provider_slug: ambient-mesh
scheme_count: 0
schemes: []
slug: ambient-mesh-authentication
source_filename: ambient-mesh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://ambientmesh.io/docs/security/\nprovider: Ambient Mesh\nproviderId: ambient-mesh\ndescription: >-\n  Authentication profile for Ambient Mesh. Derived from documentation, not from\n  an OpenAPI securitySchemes block — no OpenAPI exists for this provider (see\n  x-coverage in apis.yml). Two distinct planes have to be kept apart here, and\n  conflating them is the easy mistake: the CONFIGURATION plane is the operator's\n  own Kubernetes API server, and the DATA plane is workload-to-workload mTLS\n  that Ambient Mesh itself provides.\n\napi_keys: false\noauth2: false\noidc: false\nbasic_auth: false\nbearer_token: false\nmutual_tls: true\n\nplanes:\n  - plane: configuration\n    endpoint: the operator's own Kubernetes API server\n    provided_by: Kubernetes, not Ambient Mesh\n    scheme: >-\n      kubeconfig credential (client certificate, token, or cloud-provider\n      exec plugin) plus Kubernetes RBAC on the Istio and\
  \ Gateway API resource\n      groups. Ambient Mesh ships no credential of its own, issues no API key,\n      and hosts no authorization server.\n    evidence: >-\n      Every documented write in the docs is `kubectl`, `helm` or `istioctl`\n      against a cluster context — see https://ambientmesh.io/docs/setup/install/\n      and https://ambientmesh.io/docs/operations/upgrade/.\n  - plane: data\n    endpoint: workload-to-workload traffic inside the mesh\n    provided_by: Ambient Mesh (ztunnel and waypoint proxies)\n    scheme: mutualTLS\n    identity: SPIFFE workload identity\n    detail: >-\n      \"Ambient mesh automatically secures workload communication with mTLS as\n      soon as workloads are added to the mesh\" — no application change, no\n      sidecar injection. Certificates are issued and rotated by istiod; SPIRE\n      integration is documented for external identity issuance.\n    transport: >-\n      HBONE — HTTP CONNECT tunnels over HTTP/2, secured with mTLS, conventionally\n\
  \      on port 15008.\n    evidence:\n      - https://ambientmesh.io/docs/security/verify-mtls/\n      - https://ambientmesh.io/docs/about/key-concepts/\n  - plane: control (xDS)\n    endpoint: istiod to ztunnel / waypoints\n    provided_by: Ambient Mesh\n    scheme: mutualTLS\n    detail: >-\n      xDS configuration is delivered from istiod to the ambient data-plane\n      proxies. For multicluster, Solo Enterprise for Istio peers each cluster's\n      istiod \"over mTLS-secured xDS, without requiring remote Kubernetes API\n      access or shared kubeconfig secrets.\"\n    evidence: https://ambientmesh.io/docs/setup/requirements/\n\nauthorization:\n  - layer: L4\n    enforced_by: ztunnel\n    resource: AuthorizationPolicy (security.istio.io)\n    detail: >-\n      \"The ztunnel proxy enforces authorization policy at Layer 4 (L4). Because\n      ztunnel operates at L4,\" L7 conditions require a waypoint.\n    docs: https://ambientmesh.io/docs/security/ztunnel-authz/\n  - layer: L7\n  \
  \  enforced_by: waypoint proxy\n    resource: AuthorizationPolicy (security.istio.io)\n    detail: >-\n      \"Without a waypoint installed, you can only use Layer 4 security policies.\n      A waypoint gives you\" L7 policy — HTTP method, path and header conditions.\n    docs: https://ambientmesh.io/docs/security/waypoint-authz/\n  - layer: kubernetes\n    enforced_by: CNI plugin\n    resource: NetworkPolicy / CiliumNetworkPolicy\n    detail: >-\n      Kubernetes NetworkPolicy remains in force alongside mesh policy and has\n      documented interactions with the ambient data plane.\n    docs: https://ambientmesh.io/docs/security/configure-networkpolicies/\n\nscopes:\n  applicable: false\n  note: >-\n    No OAuth scope surface exists, so no scopes/ artifact is written.\n    Authorization is expressed as Kubernetes RBAC on the configuration plane and\n    as AuthorizationPolicy resources on the data plane.\n\nwell_known:\n  openid_configuration: 404\n  oauth_authorization_server: 404\n\
  \  see: well-known/ambient-mesh-well-known.yml\n\ndocs:\n  - https://ambientmesh.io/docs/security/\n  - https://ambientmesh.io/docs/security/verify-mtls/\n  - https://ambientmesh.io/docs/security/ztunnel-authz/\n  - https://ambientmesh.io/docs/security/waypoint-authz/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ambient-mesh/refs/heads/main/authentication/ambient-mesh-authentication.yml
summary_line: 0 schemes
tags:
- Service Mesh
- Istio
- Kubernetes
- Zero Trust
- Observability
- Traffic Management
- Microservices
---
