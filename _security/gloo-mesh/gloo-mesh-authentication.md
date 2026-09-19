---
anonymous_access: true
api_key_in: []
auth_types:
- kubernetes-rbac
- mutual-tls
- license-key
- oidc
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Gloo Mesh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gloo Mesh secures its APIs with kubernetes-rbac, mutual-tls, license-key, and oidc across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gloo Mesh
provider_slug: gloo-mesh
scheme_count: 5
schemes:
- applies_to: every Gloo custom resource in the 13 CRD API groups
  description: Clients (kubectl, Helm, meshctl, Argo CD, any controller) authenticate to the Kubernetes API server with the cluster's own mechanism and are authorized by Role / ClusterRole bindings on the Gloo CRD groups. Solo documents how to scope user access to Gloo resources and publishes the permissions the Gloo components themselves require.
  docs:
  - https://docs.solo.io/gloo-mesh-enterprise/latest/setup/prod/resource-control/
  - https://docs.solo.io/gloo-mesh-enterprise/latest/reference/permissions/
  name: Kubernetes RBAC (primary)
  type: kubernetes-rbac
- applies_to: management server <-> workload cluster agent (the relay channel)
  description: Agents authenticate to the management server with client certificates over mTLS. Solo documents five postures — self-signed certs with managed client certs, BYO server cert with managed client cert, BYO server and client certs, TLS-only, and an insecure test mode — plus a relay identity token secret and full certificate-rotation guidance, with OpenSSL, AWS Private CA and HashiCorp Vault integrations.
  docs: https://docs.solo.io/gloo-mesh-enterprise/latest/setup/prod/certs/relay/
  name: Relay mTLS
  secrets:
  - relay-root-tls-secret
  - relay-tls-signing-secret
  - relay-server-tls-secret
  - relay-identity-token-secret
  type: mutualTLS
- applies_to: feature entitlement, not request authentication
  description: A Solo-issued license key is supplied through Helm values (license.value or license.secretRef) or the Gloo istiod chart. Resources the license does not cover report ApprovalState UNLICENSED on their status rather than failing authentication. `meshctl license check` inspects it.
  docs: https://docs.solo.io/gloo-mesh-enterprise/latest/setup/prepare/licensing/
  name: Product license key
  type: license-key
- applies_to: the Gloo UI / dashboard
  description: The Gloo UI can be fronted by the customer's own OIDC identity provider. The issuer, client and callback are the customer's, which is why no OIDC discovery document is served on any solo.io host (see well-known/gloo-mesh-well-known.yml).
  docs: https://docs.solo.io/gloo-mesh-enterprise/latest/observability/tools/ui/auth/overview/
  name: OIDC for the Gloo UI
  type: openIdConnect
- applies_to: https://search.solo.io/mcp
  description: 'Probed 2026-09-12: initialize and tools/list both return 200 with no credential and the published connection instructions state "No authentication required".'
  name: Docs MCP server
  type: none
slug: gloo-mesh-authentication
source_filename: gloo-mesh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: >-\n  https://docs.solo.io/gloo-mesh-enterprise/latest/setup/prod/resource-control/ ,\n  https://docs.solo.io/gloo-mesh-enterprise/latest/setup/prod/certs/relay/ ,\n  https://docs.solo.io/gloo-mesh-enterprise/latest/setup/prepare/licensing/ ,\n  https://docs.solo.io/gloo-mesh-enterprise/latest/reference/permissions/\ndocs: https://docs.solo.io/gloo-mesh-enterprise/latest/setup/prod/resource-control/\nnote: >-\n  There is no Solo.io-operated API endpoint to obtain a key for. Gloo Mesh runs entirely in\n  the customer's own Kubernetes clusters, so the identity plane is Kubernetes': you\n  authenticate to YOUR cluster and Kubernetes RBAC decides what Gloo custom resources you may\n  read or write. The provider-issued credential is a product LICENSE key, which gates\n  features rather than access. The one Solo.io-hosted endpoint in this record, the Docs MCP\n  server, requires no authentication at all.\nsummary:\n  types: [kubernetes-rbac,\
  \ mutual-tls, license-key, oidc]\n  api_key_in: []\n  oauth2_flows: []\n  provider_hosted_auth_endpoint: false\nschemes:\n  - name: Kubernetes RBAC (primary)\n    type: kubernetes-rbac\n    applies_to: every Gloo custom resource in the 13 CRD API groups\n    description: >-\n      Clients (kubectl, Helm, meshctl, Argo CD, any controller) authenticate to the\n      Kubernetes API server with the cluster's own mechanism and are authorized by Role /\n      ClusterRole bindings on the Gloo CRD groups. Solo documents how to scope user access to\n      Gloo resources and publishes the permissions the Gloo components themselves require.\n    docs:\n      - https://docs.solo.io/gloo-mesh-enterprise/latest/setup/prod/resource-control/\n      - https://docs.solo.io/gloo-mesh-enterprise/latest/reference/permissions/\n  - name: Relay mTLS\n    type: mutualTLS\n    applies_to: management server <-> workload cluster agent (the relay channel)\n    description: >-\n      Agents authenticate to the management\
  \ server with client certificates over mTLS. Solo\n      documents five postures — self-signed certs with managed client certs, BYO server cert\n      with managed client cert, BYO server and client certs, TLS-only, and an insecure test\n      mode — plus a relay identity token secret and full certificate-rotation guidance, with\n      OpenSSL, AWS Private CA and HashiCorp Vault integrations.\n    secrets:\n      - relay-root-tls-secret\n      - relay-tls-signing-secret\n      - relay-server-tls-secret\n      - relay-identity-token-secret\n    docs: https://docs.solo.io/gloo-mesh-enterprise/latest/setup/prod/certs/relay/\n  - name: Product license key\n    type: license-key\n    applies_to: feature entitlement, not request authentication\n    description: >-\n      A Solo-issued license key is supplied through Helm values (license.value or\n      license.secretRef) or the Gloo istiod chart. Resources the license does not cover report\n      ApprovalState UNLICENSED on their status rather\
  \ than failing authentication.\n      `meshctl license check` inspects it.\n    docs: https://docs.solo.io/gloo-mesh-enterprise/latest/setup/prepare/licensing/\n  - name: OIDC for the Gloo UI\n    type: openIdConnect\n    applies_to: the Gloo UI / dashboard\n    description: >-\n      The Gloo UI can be fronted by the customer's own OIDC identity provider. The issuer,\n      client and callback are the customer's, which is why no OIDC discovery document is\n      served on any solo.io host (see well-known/gloo-mesh-well-known.yml).\n    docs: https://docs.solo.io/gloo-mesh-enterprise/latest/observability/tools/ui/auth/overview/\n  - name: Docs MCP server\n    type: none\n    applies_to: https://search.solo.io/mcp\n    description: >-\n      Probed 2026-09-12: initialize and tools/list both return 200 with no credential and the\n      published connection instructions state \"No authentication required\".\nmesh_traffic_auth:\n  note: >-\n    Distinct from authenticating TO Gloo Mesh: these\
  \ are the authN/authZ mechanisms Gloo Mesh\n    CONFIGURES for the traffic it governs, expressed as CRDs and captured in crd/.\n  mechanisms:\n    - Workload mTLS and SPIFFE identity (RootTrustPolicy, IssuedCertificate, SpireRegistrationEntry)\n    - JWT validation and claim/scope-based authorization (JWTPolicy)\n    - External auth — API keys, LDAP, OIDC, OPA, multi-step (ExtAuthPolicy, ExtAuthServer, AuthConfig)\n    - Request authorization between workloads (AccessPolicy)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gloo-mesh/refs/heads/main/authentication/gloo-mesh-authentication.yml
summary_line: kubernetes-rbac/mutual-tls/license-key/oidc · 5 schemes
tags:
- Istio
- Kubernetes
- Multi-Cluster
- Open-Source
- Service Mesh
- Envoy
- Kubernetes CRDs
- Protobuf
- Policy Enforcement
- Observability
---
