---
api_key_in: []
api_specs:
- filename: inrupt-discovery-api-openapi.yml
  format: yaml
  label: Inrupt Discovery API
  slug: inrupt-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrupt/refs/heads/main/openapi/inrupt-discovery-api-openapi.yml
- filename: inrupt-jsonkeys-api-openapi.yml
  format: yaml
  label: Inrupt Jsonkeys API
  slug: inrupt-jsonkeys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrupt/refs/heads/main/openapi/inrupt-jsonkeys-api-openapi.yml
- filename: inrupt-subscription-api-openapi.yml
  format: yaml
  label: Inrupt Subscription API
  slug: inrupt-subscription-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inrupt/refs/heads/main/openapi/inrupt-subscription-api-openapi.yml
auth_types:
- openIdConnect
- oauth2
- http
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Inrupt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Inrupt secures its APIs with openIdConnect, oauth2, http, and mutualTLS across 7 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Inrupt
provider_slug: inrupt
scheme_count: 7
schemes:
- bearerFormat: JWT
  description: The security scheme declared in the published Notification Delivery Service OpenAPI. It is applied per-operation on every /subscriptions and /system/subscriptions operation; the discovery (POST /) and JWKS (GET /jwks) operations are unauthenticated.
  name: SolidAuthentication
  scheme: bearer
  sources:
  - openapi/inrupt-notification-openapi.yaml
  type: http
- claims:
  - sub
  - webid
  - iss
  - aud
  description: Hosted Solid OpenID Provider for PodSpaces WebIDs. Supports authorization_code (with PKCE S256), refresh_token and client_credentials, dynamic client registration, revocation and end-session.
  id_token_signing_algs:
  - RS256
  - ES256
  issuer: https://login.inrupt.com
  name: SolidOIDC
  openIdConnectUrl: https://login.inrupt.com/.well-known/openid-configuration
  scopes:
  - openid
  - offline_access
  - webid
  sources:
  - https://login.inrupt.com/.well-known/openid-configuration
  type: openIdConnect
- description: 'Demonstrating Proof of Possession (RFC 9449). The provider advertises dpop_signing_alg_values_supported [RS256, ES256]; ESS request examples use "Authorization: DPoP <token>" together with a "DPoP: <proof>" header, which binds the token to the client key so a stolen bearer token is not enough.'
  name: DPoP
  sources:
  - https://login.inrupt.com/.well-known/openid-configuration
  - https://docs.inrupt.com/ess/services/service-pod-management/data-views-api
  type: oauth2
- description: ESS 3.0 native IdP support. A client authenticates with its own external OIDC Identity Provider, then exchanges the resulting id_token (subject_token_type urn:ietf:params:oauth:token-type:id_token) for an ESS Access Token. The issuer must be on the deployment's trusted-issuer allow list. Default token TTL is 5 minutes; clients should re-exchange proactively using expires_in and retry once on 401.
  endpoint: https://platform.{ess-domain}/access/token
  flow: urn:ietf:params:oauth:grant-type:token-exchange
  name: TokenExchange
  sources:
  - https://docs.inrupt.com/ess/services/service-platform-management/token-exchange
  - https://docs.inrupt.com/guides/integrating-with-ess-mcp
  type: oauth2
- description: Server-side applications authenticate as themselves (a single-user or service application) using client credentials registered with the identity provider.
  flow: clientCredentials
  name: ClientCredentials
  sources:
  - https://docs.inrupt.com/guides/authentication-in-solid/authentication-server-side
  - https://docs.inrupt.com/sdk/java-sdk/authentication/session-management
  type: oauth2
- description: Solid-OIDC Client Identifier Documents - a client is identified by a dereferenceable URI hosting a JSON-LD Client ID Document rather than by a registered client_id string. ESS deployments maintain allow lists of client IDs for authorization and initial Pod access.
  name: ClientIdDocument
  sources:
  - https://docs.inrupt.com/guides/identity-in-solid/the-client-id-document
  - https://docs.inrupt.com/sdk/java-sdk/authentication/solid-oidc-client-identifiers
  type: openIdConnect
- description: Outbound only. A notification subscription may carry dispatch.authentication of type mtls with a PEM-formatted X.509 serverCertificate, so the Notification Delivery Service can authenticate the subscriber's webhook endpoint.
  name: WebhookMutualTLS
  sources:
  - openapi/inrupt-notification-openapi.yaml
  - https://docs.inrupt.com/ess/services/service-notification/notification-delivery-service
  type: mutualTLS
slug: inrupt-authentication
source_filename: inrupt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: >-\n  https://login.inrupt.com/.well-known/openid-configuration (probed),\n  openapi/inrupt-notification-openapi.yaml (derived),\n  https://docs.inrupt.com/guides/authentication-in-solid,\n  https://docs.inrupt.com/security/authentication,\n  https://docs.inrupt.com/ess/services/service-platform-management/token-exchange\ndocs: https://docs.inrupt.com/security/authentication\nsummary:\n  types:\n  - openIdConnect\n  - oauth2\n  - http\n  - mutualTLS\n  primary: Solid-OIDC bearer tokens, DPoP-bound where the deployment requires proof of possession.\nschemes:\n- name: SolidAuthentication\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/inrupt-notification-openapi.yaml\n  description: >-\n    The security scheme declared in the published Notification Delivery Service OpenAPI. It is applied\n    per-operation on every /subscriptions and /system/subscriptions operation; the discovery (POST /)\n    and\
  \ JWKS (GET /jwks) operations are unauthenticated.\n- name: SolidOIDC\n  type: openIdConnect\n  openIdConnectUrl: https://login.inrupt.com/.well-known/openid-configuration\n  issuer: https://login.inrupt.com\n  sources:\n  - https://login.inrupt.com/.well-known/openid-configuration\n  description: >-\n    Hosted Solid OpenID Provider for PodSpaces WebIDs. Supports authorization_code (with PKCE S256),\n    refresh_token and client_credentials, dynamic client registration, revocation and end-session.\n  scopes:\n  - openid\n  - offline_access\n  - webid\n  claims:\n  - sub\n  - webid\n  - iss\n  - aud\n  id_token_signing_algs:\n  - RS256\n  - ES256\n- name: DPoP\n  type: oauth2\n  description: >-\n    Demonstrating Proof of Possession (RFC 9449). The provider advertises\n    dpop_signing_alg_values_supported [RS256, ES256]; ESS request examples use\n    \"Authorization: DPoP <token>\" together with a \"DPoP: <proof>\" header, which binds the token to the\n    client key so a stolen bearer\
  \ token is not enough.\n  sources:\n  - https://login.inrupt.com/.well-known/openid-configuration\n  - https://docs.inrupt.com/ess/services/service-pod-management/data-views-api\n- name: TokenExchange\n  type: oauth2\n  flow: urn:ietf:params:oauth:grant-type:token-exchange\n  endpoint: https://platform.{ess-domain}/access/token\n  description: >-\n    ESS 3.0 native IdP support. A client authenticates with its own external OIDC Identity Provider,\n    then exchanges the resulting id_token (subject_token_type\n    urn:ietf:params:oauth:token-type:id_token) for an ESS Access Token. The issuer must be on the\n    deployment's trusted-issuer allow list. Default token TTL is 5 minutes; clients should re-exchange\n    proactively using expires_in and retry once on 401.\n  sources:\n  - https://docs.inrupt.com/ess/services/service-platform-management/token-exchange\n  - https://docs.inrupt.com/guides/integrating-with-ess-mcp\n- name: ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n\
  \  description: >-\n    Server-side applications authenticate as themselves (a single-user or service application) using\n    client credentials registered with the identity provider.\n  sources:\n  - https://docs.inrupt.com/guides/authentication-in-solid/authentication-server-side\n  - https://docs.inrupt.com/sdk/java-sdk/authentication/session-management\n- name: ClientIdDocument\n  type: openIdConnect\n  description: >-\n    Solid-OIDC Client Identifier Documents - a client is identified by a dereferenceable URI hosting a\n    JSON-LD Client ID Document rather than by a registered client_id string. ESS deployments maintain\n    allow lists of client IDs for authorization and initial Pod access.\n  sources:\n  - https://docs.inrupt.com/guides/identity-in-solid/the-client-id-document\n  - https://docs.inrupt.com/sdk/java-sdk/authentication/solid-oidc-client-identifiers\n- name: WebhookMutualTLS\n  type: mutualTLS\n  description: >-\n    Outbound only. A notification subscription may carry\
  \ dispatch.authentication of type mtls with a\n    PEM-formatted X.509 serverCertificate, so the Notification Delivery Service can authenticate the\n    subscriber's webhook endpoint.\n  sources:\n  - openapi/inrupt-notification-openapi.yaml\n  - https://docs.inrupt.com/ess/services/service-notification/notification-delivery-service\noutbound_message_authentication:\n  standard: RFC 9421 HTTP Message Signatures\n  keys: https://notification.{ess-domain}/jwks\n  description: >-\n    Webhooks receive signed requests; the receiver verifies with the published JWK Set before\n    processing. This is the reverse direction of the schemes above and is required, not optional.\nauthorization_note: >-\n  Authentication establishes a WebID. Authorization is separate - see scopes/inrupt-scopes.yml for the\n  ACP + Access Grant model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inrupt/refs/heads/main/authentication/inrupt-authentication.yml
summary_line: openIdConnect/oauth2/http/mutualTLS · 7 schemes
tags:
- Company
- Solid
- Personal Data Stores
- Decentralized Identity
- Data Privacy
- Access Control
- Verifiable Credentials
- Linked Data
- RDF
- Consent Management
- Data Wallets
- Agent Infrastructure
- MCP
- Enterprise Software
---
