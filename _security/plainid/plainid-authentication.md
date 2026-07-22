---
api_key_in:
- header
- body
auth_types:
- apiKey
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Plainid Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- tokenExchange
overview: PlainID secures its APIs with apiKey, oauth2, and http across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and tokenExchange flow(s).
provider_name: PlainID
provider_slug: plainid
scheme_count: 3
schemes:
- alt_location: request body (clientId, clientSecret)
  description: Runtime Authorization (PDP) API credentials. clientId and entityId are mandatory on every runtime call even when a JWT is also supplied.
  in: header
  name: RuntimeClientCredentials
  parameters:
  - X-Client-Id
  - X-Client-Secret
  required_fields:
  - clientId
  - entityId
  source: https://docs.plainid.io/apidocs/authentication-1.md
  surface: runtime
  type: apiKey
- bearerFormat: JWT
  description: Optional identity JWT verified against the issuer JWKS URL configured under Tenant Management > Policy Authorization Agents. Supplies identity attributes for the access decision; invalid JWTs yield no attributes.
  name: RuntimeJWTBearer
  scheme: bearer
  source: https://docs.plainid.io/apidocs/authentication-1.md
  surface: runtime
  type: http
- description: OAuth 2.0 Client Credentials flow against the tenant Keycloak realm. Client credentials are created at the Tenant or Environment level and replace the legacy IDP token-exchange flow. The returned token is sent as an Authorization Bearer header on Management and Administration API calls.
  flow: clientCredentials
  name: ManagementClientCredentials
  source: https://docs.plainid.io/apidocs/authentication-mgmt-apis.md
  surface: management
  token_type: Bearer
  token_url: https://auth.<base-plainid-url>/auth/realms/<tenant-subdomain>/protocol/openid-connect/token
  type: oauth2
slug: plainid-authentication
source_filename: plainid-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.plainid.io/apidocs/authentication-1.md\ndocs:\n  runtime: https://docs.plainid.io/apidocs/authentication-1.md\n  management: https://docs.plainid.io/apidocs/authentication-mgmt-apis.md\n  token_exchange: https://docs.plainid.io/apidocs/about-token-exchange.md\nsummary:\n  types: [apiKey, oauth2, http]\n  api_key_in: [header, body]\n  oauth2_flows: [clientCredentials, tokenExchange]\n  notes: >-\n    PlainID exposes two authentication surfaces. Runtime (PDP) Authorization\n    APIs authenticate with a clientId/clientSecret pair (request body or the\n    X-Client-Id / X-Client-Secret headers) or a JWT bearer token verified\n    against the configured issuer JWKS. Management / Administration APIs use an\n    OAuth 2.0 Client Credentials flow (which replaces the older IDP token-exchange\n    flow) against the tenant Keycloak realm, returning a Bearer access token.\nschemes:\n  - name: RuntimeClientCredentials\n   \
  \ surface: runtime\n    type: apiKey\n    in: header\n    parameters: [X-Client-Id, X-Client-Secret]\n    alt_location: request body (clientId, clientSecret)\n    required_fields: [clientId, entityId]\n    description: >-\n      Runtime Authorization (PDP) API credentials. clientId and entityId are\n      mandatory on every runtime call even when a JWT is also supplied.\n    source: https://docs.plainid.io/apidocs/authentication-1.md\n  - name: RuntimeJWTBearer\n    surface: runtime\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Optional identity JWT verified against the issuer JWKS URL configured under\n      Tenant Management > Policy Authorization Agents. Supplies identity\n      attributes for the access decision; invalid JWTs yield no attributes.\n    source: https://docs.plainid.io/apidocs/authentication-1.md\n  - name: ManagementClientCredentials\n    surface: management\n    type: oauth2\n    flow: clientCredentials\n    token_url: https://auth.<base-plainid-url>/auth/realms/<tenant-subdomain>/protocol/openid-connect/token\n\
  \    token_type: Bearer\n    description: >-\n      OAuth 2.0 Client Credentials flow against the tenant Keycloak realm.\n      Client credentials are created at the Tenant or Environment level and\n      replace the legacy IDP token-exchange flow. The returned token is sent as\n      an Authorization Bearer header on Management and Administration API calls.\n    source: https://docs.plainid.io/apidocs/authentication-mgmt-apis.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/plainid/refs/heads/main/authentication/plainid-authentication.yml
summary_line: apiKey/oauth2/http · 3 schemes
tags:
- Company
- Cybersecurity
- Authorization
- Access Control
- PBAC
- Identity
- Policy Management
- API Security
---
