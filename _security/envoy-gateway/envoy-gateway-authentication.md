---
anonymous_access: false
api_key_in: []
auth_types: []
description: Two different things are easy to confuse here, and conflating them would misdescribe the product. Envoy Gateway has no credential of its own — you authenticate to the Kubernetes API server and RBAC decides whether you may write its resources. What it PROVIDES is a rich authentication surface for the traffic passing through the gateway, configured through SecurityPolicy. The first is this artifact's `provider` section; the second is its `provided` section, and only the first describes how a consumer gets in.
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Envoy Gateway Authentication
name_suffix: Authentication
oauth_flows: []
overview: Envoy Gateway declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Envoy Gateway
provider_slug: envoy-gateway
scheme_count: 0
schemes: []
slug: envoy-gateway-authentication
source_filename: envoy-gateway-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Envoy Gateway\nproviderId: envoy-gateway\ngenerated: '2026-09-07'\nmethod: searched\nsource: >-\n  https://gateway.envoyproxy.io/docs/tasks/security/ and the SecurityPolicy and\n  ClientTrafficPolicy schemas in json-schema/envoy-gateway-crds.yaml.\n  derive-authentication.py was run first and returned no profile, correctly: it reads\n  OpenAPI securitySchemes and this provider publishes no OpenAPI.\ndescription: >-\n  Two different things are easy to confuse here, and conflating them would misdescribe the\n  product. Envoy Gateway has no credential of its own — you authenticate to the Kubernetes\n  API server and RBAC decides whether you may write its resources. What it PROVIDES is a\n  rich authentication surface for the traffic passing through the gateway, configured\n  through SecurityPolicy. The first is this artifact's `provider` section; the second is\n  its `provided` section, and only\
  \ the first describes how a consumer gets in.\nprovider:\n  schemes:\n    - type: kubernetes\n      name: Kubernetes API server authentication\n      description: >-\n        Client certificates, bearer tokens, OIDC, or a cloud provider's IAM authenticator —\n        whatever the cluster is configured for. Envoy Gateway inherits it entirely.\n      authorization: >-\n        Kubernetes RBAC on the gateway.envoyproxy.io API group. A Role or ClusterRole\n        granting verbs on backends, backendtrafficpolicies, clienttrafficpolicies,\n        envoyextensionpolicies, envoypatchpolicies, envoyproxies, httproutefilters and\n        securitypolicies is what actually gates access.\n      note: Nothing is issued by Envoy Gateway. There is no API key, token or console login.\n    - type: mutualTLS\n      name: xDS control plane to data plane\n      description: >-\n        The control plane serves xDS to the managed Envoy proxies over mTLS, with\n        certificates provisioned by the certgen\
  \ Job or by cert-manager. Operators do not\n        call this channel; it is internal.\n      note: >-\n        v1.9.0 fixed an authentication bypass on this channel in GatewayNamespaceMode —\n        see security/envoy-gateway-vulnerability-disclosure.yml.\n  oauth2: false\n  apiKey: false\n  scopes: null\n  scopesNote: >-\n    No OAuth scopes artifact is written. derive-oauth-scopes.py found no oauth2\n    securityScheme because there is no spec, and the real authorization model is RBAC verbs\n    on Kubernetes resources, which is not a scope list.\nprovided:\n  description: >-\n    Authentication methods Envoy Gateway can enforce on traffic traversing the gateway,\n    all configured on the SecurityPolicy CRD. Listed because for this product they are the\n    feature a buyer is shopping for.\n  crd: SecurityPolicy\n  docs: https://gateway.envoyproxy.io/docs/api/extension_types/#securitypolicy\n  methods:\n    - field: spec.jwt\n      name: JWT validation\n      detail: >-\n        Per-provider\
  \ issuers, audiences, remote or local JWKS, claim-to-header extraction,\n        failedRefetchDuration and (v1.9.0) failOpen.\n    - field: spec.oidc\n      name: OpenID Connect\n      detail: >-\n        Authorization-code flow with PKCE, discovery, refresh, logout, and forwardIDToken\n        (v1.9.0). v1.9.1 removed HTTP as an acceptable issuer scheme and moved session\n        cookies to AES-256-GCM.\n    - field: spec.apiKeyAuth\n      name: API key authentication\n      detail: >-\n        Keys extracted from headers, query parameters or cookies. v1.9.0 tightened\n        extractFrom validation to require at least one entry naming exactly one source.\n    - field: spec.basicAuth\n      name: HTTP Basic authentication\n      detail: Credentials from a Kubernetes Secret containing an htpasswd file.\n    - field: spec.extAuth\n      name: External authorization\n      detail: Delegates the decision to an HTTP or gRPC external authorization service.\n    - field: spec.authorization\n\
  \      name: Authorization rules\n      detail: >-\n        Allow/deny rules on client CIDR, JWT claims, headers and (v1.9.0) CEL expressions\n        and path matches.\n    - field: ClientTrafficPolicy spec.tls.clientValidation\n      name: Mutual TLS for downstream clients\n      detail: >-\n        CA certificate refs, optional insecure fallback, and (v1.9.0)\n        allowExpiredCertificate.\n    - field: spec.csrf\n      name: CSRF protection\n      detail: >-\n        Added v1.9.0. Validates the Origin header of mutating requests against the\n        destination and additionalOrigins, with gradual rollout via shadowFraction.\n    - field: spec.cors\n      name: CORS\n      detail: Cross-origin request handling at the gateway.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/envoy-gateway/refs/heads/main/authentication/envoy-gateway-authentication.yml
summary_line: 0 schemes
tags:
- API Gateway
- CNCF
- Envoy
- Kubernetes
- Open-Source
- Gateway API
- Ingress
- Service Mesh
- Cloud Native
- gRPC
---
