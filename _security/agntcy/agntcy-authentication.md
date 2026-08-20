---
api_key_in:
- header
api_specs:
- filename: agntcy-oasf-schema-swagger.json
  format: json
  label: OASF Schema API
  slug: oasf-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agntcy/refs/heads/main/openapi/agntcy-oasf-schema-swagger.json
- filename: agntcy-acp-openapi.json
  format: json
  label: Agent Connect Protocol (ACP)
  slug: agent-connect-protocol-acp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agntcy/refs/heads/main/openapi/agntcy-acp-openapi.json
- filename: agntcy-identity-service-openapi.yaml
  format: yaml
  label: AGNTCY Identity Service API
  slug: agntcy-identity-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agntcy/refs/heads/main/openapi/agntcy-identity-service-openapi.yaml
- filename: agntcy-identity-node-openapi.yaml
  format: yaml
  label: AGNTCY Identity Node API
  slug: agntcy-identity-node-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agntcy/refs/heads/main/openapi/agntcy-identity-node-openapi.yaml
auth_types:
- apiKey
- http
- openIdConnect
- mutualTLS
- none
description: ''
kind: authentication
layout: security
method: searched
name: Agntcy Authentication
name_suffix: Authentication
oauth_flows: []
overview: AGNTCY secures its APIs with apiKey, http, openIdConnect, mutualTLS, and none across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AGNTCY
provider_slug: agntcy
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: An IAM JWT token issued to a user during an OIDC flow.
  name: AccessToken
  scheme: bearer
  sources:
  - openapi/agntcy-identity-service-openapi.yaml
  type: http
- description: An IAM Api key.
  in: header
  name: ApiKey
  parameter: x-id-api-key
  sources:
  - openapi/agntcy-identity-service-openapi.yaml
  type: apiKey
slug: agntcy-authentication
source_filename: agntcy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: searched\nsource: openapi/agntcy-identity-service-openapi.yaml plus the AGNTCY Directory authentication documentation\nsummary:\n  types:\n  - apiKey\n  - http\n  - openIdConnect\n  - mutualTLS\n  - none\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: AccessToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: An IAM JWT token issued to a user during an OIDC flow.\n  sources:\n  - openapi/agntcy-identity-service-openapi.yaml\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: x-id-api-key\n  description: An IAM Api key.\n  sources:\n  - openapi/agntcy-identity-service-openapi.yaml\ndocs: https://github.com/agntcy/dir/blob/main/docs/content/dir/dir-component-oidc-authentication.md\nnote: AGNTCY has four independent auth models, only one of which appears in an OpenAPI. The two schemes below are derived\n  from the Identity Service spec; the surfaces block records the rest, which are documented in\
  \ prose only. No oauth2 securityScheme\n  is declared in any published spec, so no scopes/ artifact is emitted even though OIDC is used.\nsurfaces:\n- surface: OASF Schema API\n  host: https://schema.oasf.outshift.com\n  auth: none\n  evidence: openapi/agntcy-oasf-schema-swagger.json declares no securityDefinitions; live GET /api/versions returned 200 anonymously\n    on 2026-08-19\n- surface: AGNTCY Identity Service\n  auth:\n  - bearer-jwt\n  - api-key\n  schemes:\n  - 'AccessToken (Authorization: Bearer <IAM JWT issued during an OIDC flow)'\n  - ApiKey (x-id-api-key header)\n  token_flow:\n  - AuthService_Authorize\n  - AuthService_Token\n  key_rotation: AppService_RefreshAppApiKey\n  evidence: openapi/agntcy-identity-service-openapi.yaml components.securitySchemes\n- surface: AGNTCY Identity Node\n  auth: none-declared\n  evidence: openapi/agntcy-identity-node-openapi.yaml declares no securitySchemes; the node is self-hosted and fronted by\n    the operator\n- surface: Agent Directory\
  \ (DIR)\n  auth:\n  - spiffe-x509\n  - spiffe-jwt\n  - spiffe-token\n  - mtls\n  - oidc\n  - insecure\n  - none\n  default: auto-detect (OIDC if a cached token, issuer or client id is present; falls back to insecure for local development)\n  primary_trust_model: SPIFFE/SPIRE for in-cluster workload and service-to-service identity\n  external_access: optional oidc-gateway (Envoy) accepting OIDC JWT, SPIFFE JWT-SVID and SPIFFE X.509-SVID, able to expose\n    OIDC/JWT and X.509-SVID mTLS on separate hostnames\n  client_env:\n  - DIRECTORY_CLIENT_AUTH_MODE\n  - DIRECTORY_CLIENT_AUTH_TOKEN\n  - DIRECTORY_CLIENT_OIDC_ISSUER\n  - DIRECTORY_CLIENT_OIDC_CLIENT_ID\n  - DIRECTORY_CLIENT_SPIFFE_SOCKET_PATH\n  - DIRECTORY_CLIENT_JWT_AUDIENCE\n  - DIRECTORY_CLIENT_TLS_CERT_FILE\n  - DIRECTORY_CLIENT_TLS_KEY_FILE\n  - DIRECTORY_CLIENT_TLS_CA_FILE\n  interactive_login: dirctl auth login --oidc-issuer <url> --oidc-client-id dirctl (PKCE, --no-browser or --device); tokens\n    cached issuer-scoped under\
  \ ~/.config/dirctl/tokens/\n  ci: 'GitHub Actions OIDC via --oidc-audience with job permission id-token: write; dirctl mints and renews its own tokens'\n  tested_idps:\n  - Zitadel\n  - Keycloak\n  - Auth0\n  - Okta\n  - Microsoft Entra ID\n  - Dex\n  evidence: https://github.com/agntcy/dir/blob/main/docs/content/dir/dir-component-oidc-authentication.md and dir-cli-reference.md\n- surface: Agent Connect Protocol\n  auth: implementation-defined\n  evidence: openapi/agntcy-acp-openapi.json declares no securitySchemes and no servers[]; ACP is an interface each agent server\n    implements under its own auth\nwell_known_jwks:\n  served_by: AGNTCY Identity Node and by any domain publishing record names\n  operations:\n  - IssuerService_GetWellKnown (/v1alpha1/issuer/{commonName}/.well-known/jwks.json)\n  - VcService_GetWellKnown (/v1alpha1/vc/{id}/.well-known/vcs.json)\n  note: Directory name verification reads a claimed domain /.well-known/jwks.json to prove ownership of a URL-based record\n\
  \    name. AGNTCY defines these paths but serves none of them itself.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agntcy/refs/heads/main/authentication/agntcy-authentication.yml
summary_line: apiKey/http/openIdConnect/mutualTLS/none · 2 schemes
tags:
- AI Agents
- Interoperability
- Specification
- Open-Source
- Agent Discovery
- Identity
- Agent Directory
- MCP
- A2A
- OpenAPI
- gRPC
- Protocol Buffers
- Verifiable Credentials
- Schema
- Taxonomy
- Messaging
- Observability
- Linux Foundation
---
