---
api_key_in: []
api_specs:
- filename: virtru-authorization-openapi.yaml
  format: yaml
  label: Virtru Authorization (v1)
  slug: virtru-authorization-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-authorization-openapi.yaml
- filename: virtru-authorization-v2-openapi.yaml
  format: yaml
  label: Virtru Authorization (v2)
  slug: virtru-authorization-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-authorization-v2-openapi.yaml
- filename: virtru-entity-openapi.yaml
  format: yaml
  label: Virtru Entity
  slug: virtru-entity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-entity-openapi.yaml
- filename: virtru-entity-resolution-v2-openapi.yaml
  format: yaml
  label: Virtru Entity Resolution (v2)
  slug: virtru-entity-resolution-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-entity-resolution-v2-openapi.yaml
- filename: virtru-kas-openapi.yaml
  format: yaml
  label: Virtru Key Access Service (KAS)
  slug: virtru-key-access-service-kas
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-kas-openapi.yaml
- filename: virtru-policy-actions-openapi.yaml
  format: yaml
  label: Virtru Policy — Actions
  slug: virtru-policy-actions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-actions-openapi.yaml
- filename: virtru-policy-attributes-openapi.yaml
  format: yaml
  label: Virtru Policy — Attributes
  slug: virtru-policy-attributes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-attributes-openapi.yaml
- filename: virtru-policy-kas-registry-openapi.yaml
  format: yaml
  label: Virtru Policy — KAS Registry
  slug: virtru-policy-kas-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-kas-registry-openapi.yaml
- filename: virtru-policy-key-management-openapi.yaml
  format: yaml
  label: Virtru Policy — Key Management
  slug: virtru-policy-key-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-key-management-openapi.yaml
- filename: virtru-policy-namespaces-openapi.yaml
  format: yaml
  label: Virtru Policy — Namespaces
  slug: virtru-policy-namespaces
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-namespaces-openapi.yaml
- filename: virtru-policy-obligations-openapi.yaml
  format: yaml
  label: Virtru Policy — Obligations
  slug: virtru-policy-obligations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-obligations-openapi.yaml
- filename: virtru-policy-registered-resources-openapi.yaml
  format: yaml
  label: Virtru Policy — Registered Resources
  slug: virtru-policy-registered-resources
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-registered-resources-openapi.yaml
- filename: virtru-policy-resource-mapping-openapi.yaml
  format: yaml
  label: Virtru Policy — Resource Mapping
  slug: virtru-policy-resource-mapping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-resource-mapping-openapi.yaml
- filename: virtru-policy-subject-mapping-openapi.yaml
  format: yaml
  label: Virtru Policy — Subject Mapping
  slug: virtru-policy-subject-mapping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-subject-mapping-openapi.yaml
- filename: virtru-wellknown-configuration-openapi.yaml
  format: yaml
  label: Virtru Well-Known Configuration
  slug: virtru-well-known-configuration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-wellknown-configuration-openapi.yaml
auth_types:
- oauth2
- openIdConnect
description: The Virtru Data Security Platform (OpenTDF) authenticates all service calls with OpenID Connect (OIDC) / OAuth 2.0. Clients obtain an access token from the platform's configured identity provider (Keycloak by default) and present it as a Bearer token on every Connect/gRPC request to the Policy, Key Access (KAS), Authorization, Entity Resolution and Well-Known services. Key operations additionally use PKCS#11 for HSM-backed key material and ABAC (attribute-based access control) for authorization decisions.
kind: authentication
layout: security
method: searched
name: Virtru Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Virtru secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Virtru
provider_slug: virtru
scheme_count: 3
schemes:
- description: OpenID Connect discovery via the platform Well-Known configuration service. Tokens issued by the deployment's IdP (Keycloak by default).
  name: OIDC
  sources:
  - docs
  type: openIdConnect
- flows:
  - description: Machine-to-machine service auth for SDKs and pipelines.
    flow: clientCredentials
  - description: Interactive user auth for web/console clients.
    flow: authorizationCode
  name: OAuth2
  sources:
  - docs
  type: oauth2
- description: PKCS#11 HSM interface for KAS key wrapping/unwrapping (hardware-backed key custody).
  name: PKCS11
  sources:
  - docs
  type: mutualTLS
slug: virtru-authentication
source_filename: virtru-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://www.virtru.com/developers/get-started\ndocs: https://opentdf.io/quickstart\ndescription: >-\n  The Virtru Data Security Platform (OpenTDF) authenticates all service calls with\n  OpenID Connect (OIDC) / OAuth 2.0. Clients obtain an access token from the platform's\n  configured identity provider (Keycloak by default) and present it as a Bearer token on\n  every Connect/gRPC request to the Policy, Key Access (KAS), Authorization, Entity\n  Resolution and Well-Known services. Key operations additionally use PKCS#11 for HSM-backed\n  key material and ABAC (attribute-based access control) for authorization decisions.\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [clientCredentials, authorizationCode]\nschemes:\n  - name: OIDC\n    type: openIdConnect\n    description: >-\n      OpenID Connect discovery via the platform Well-Known configuration service. Tokens\n      issued by the deployment's\
  \ IdP (Keycloak by default).\n    sources: [docs]\n  - name: OAuth2\n    type: oauth2\n    flows:\n      - flow: clientCredentials\n        description: Machine-to-machine service auth for SDKs and pipelines.\n      - flow: authorizationCode\n        description: Interactive user auth for web/console clients.\n    sources: [docs]\n  - name: PKCS11\n    type: mutualTLS\n    description: >-\n      PKCS#11 HSM interface for KAS key wrapping/unwrapping (hardware-backed key custody).\n    sources: [docs]\nnotes: >-\n  The published Connect-protocol OpenAPI specs do not declare securitySchemes inline\n  (auth is enforced at the gateway), so this profile is sourced from the OpenTDF\n  platform authentication documentation rather than derived from the spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/authentication/virtru-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Company
- Cybersecurity
- Data Security
- Encryption
- Access Control
- Zero Trust
- Data Privacy
- OpenTDF
- Key Management
---
