---
api_key_in: []
api_specs:
- filename: virtru-authorization-authorizationservice-api-openapi.yml
  format: yaml
  label: Virtru authorization.AuthorizationService API
  slug: virtru-authorization-authorizationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-authorization-authorizationservice-api-openapi.yml
- filename: virtru-authorization-v2-authorizationservice-api-openapi.yml
  format: yaml
  label: Virtru authorization.v2.AuthorizationService API
  slug: virtru-authorization-v2-authorizationservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-authorization-v2-authorizationservice-api-openapi.yml
- filename: virtru-entityresolution-v2-entityresolutionservice-api-openapi.yml
  format: yaml
  label: Virtru entityresolution.v2.EntityResolutionService API
  slug: virtru-entityresolution-v2-entityresolutionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-entityresolution-v2-entityresolutionservice-api-openapi.yml
- filename: virtru-kas-accessservice-api-openapi.yml
  format: yaml
  label: Virtru kas.AccessService API
  slug: virtru-kas-accessservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-kas-accessservice-api-openapi.yml
- filename: virtru-policy-actions-actionservice-api-openapi.yml
  format: yaml
  label: Virtru policy.actions.ActionService API
  slug: virtru-policy-actions-actionservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-actions-actionservice-api-openapi.yml
- filename: virtru-policy-attributes-attributesservice-api-openapi.yml
  format: yaml
  label: Virtru policy.attributes.AttributesService API
  slug: virtru-policy-attributes-attributesservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-attributes-attributesservice-api-openapi.yml
- filename: virtru-policy-kasregistry-keyaccessserverregistryservice-api-openapi.yml
  format: yaml
  label: Virtru policy.kasregistry.KeyAccessServerRegistryService API
  slug: virtru-policy-kasregistry-keyaccessserverregistryservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-kasregistry-keyaccessserverregistryservice-api-openapi.yml
- filename: virtru-policy-keymanagement-keymanagementservice-api-openapi.yml
  format: yaml
  label: Virtru policy.keymanagement.KeyManagementService API
  slug: virtru-policy-keymanagement-keymanagementservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-keymanagement-keymanagementservice-api-openapi.yml
- filename: virtru-policy-namespaces-namespaceservice-api-openapi.yml
  format: yaml
  label: Virtru policy.namespaces.NamespaceService API
  slug: virtru-policy-namespaces-namespaceservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-namespaces-namespaceservice-api-openapi.yml
- filename: virtru-policy-obligations-service-api-openapi.yml
  format: yaml
  label: Virtru policy.obligations.Service API
  slug: virtru-policy-obligations-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-obligations-service-api-openapi.yml
- filename: virtru-policy-registeredresources-registeredresourcesservice-api-openapi.yml
  format: yaml
  label: Virtru policy.registeredresources.RegisteredResourcesService API
  slug: virtru-policy-registeredresources-registeredresourcesservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-registeredresources-registeredresourcesservice-api-openapi.yml
- filename: virtru-policy-resourcemapping-resourcemappingservice-api-openapi.yml
  format: yaml
  label: Virtru policy.resourcemapping.ResourceMappingService API
  slug: virtru-policy-resourcemapping-resourcemappingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-resourcemapping-resourcemappingservice-api-openapi.yml
- filename: virtru-policy-subjectmapping-subjectmappingservice-api-openapi.yml
  format: yaml
  label: Virtru policy.subjectmapping.SubjectMappingService API
  slug: virtru-policy-subjectmapping-subjectmappingservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-policy-subjectmapping-subjectmappingservice-api-openapi.yml
- filename: virtru-wellknownconfiguration-wellknownservice-api-openapi.yml
  format: yaml
  label: Virtru wellknownconfiguration.WellKnownService API
  slug: virtru-wellknownconfiguration-wellknownservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/virtru/refs/heads/main/openapi/virtru-wellknownconfiguration-wellknownservice-api-openapi.yml
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
