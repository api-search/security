---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aedifion-openapi.yml
  format: yaml
  label: aedifion HTTP API
  slug: aedifion-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aedifion/refs/heads/main/openapi/aedifion-openapi.yml
- filename: aedifion-mqtt-asyncapi.yml
  format: yaml
  label: aedifion MQTT API
  slug: aedifion-mqtt-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/aedifion/refs/heads/main/asyncapi/aedifion-mqtt-asyncapi.yml
auth_types:
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Aedifion Authentication
name_suffix: Authentication
oauth_flows:
- implicit
- authorizationCode
- password
- clientCredentials
overview: Aedifion secures its APIs with http, oauth2, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the implicit, authorizationCode, password, and clientCredentials flow(s).
provider_name: Aedifion
provider_slug: aedifion
scheme_count: 4
schemes:
- header: 'Authorization: Basic base64(email:password)'
  name: basicAuth
  note: The docs state "The aedifion HTTP API supports Basic Auth for legacy reasons until further notice. HTTP Basic Auth may be deprecated in future." Credentials are the user's platform email and password, sent on every request, so it must only be used over HTTPS.
  rfc: RFC 7617
  scheme: basic
  sources:
  - openapi/aedifion-openapi.yml
  status: legacy
  type: http
- endpoints:
    authorization: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/auth
    introspection: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/token/introspect
    jwks_uri: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/certs
    token: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/token
  flows:
  - declared_in: openapi
    flow: implicit
  - declared_in: oidc-discovery
    flow: authorizationCode
  - declared_in: docs
    flow: password
    note: Keycloak Direct Access Grant - grant_type=password with client_id, username, password.
  - declared_in: oidc-discovery
    flow: clientCredentials
  header: 'Authorization: Bearer <access_token>'
  issuer: https://auth.aedifion.io/realms/aedifion
  name: openIDConnect
  provider: Keycloak
  sources:
  - openapi/aedifion-openapi.yml
  - well-known/aedifion-openid-configuration.json
  subtype: openIdConnect
  token_endpoint_auth_methods:
  - private_key_jwt
  - client_secret_basic
  - client_secret_post
  - tls_client_auth
  - client_secret_jwt
  type: oauth2
- docs: https://docs.aedifion.io/en/developers/http-api/guides-and-tutorials/mqtt-user-management/
  name: mqtt-credentials
  note: The MQTT broker at mqtt.aedifion.io authenticates with username/password in the MQTT CONNECT packet over TLS. Limited-validity credentials are minted through the HTTP API's MQTT user-management endpoints; unlimited-validity credentials are issued only on request by aedifion staff. Authorization is per-topic read/write.
  transport: mqtt
  type: other
- docs: https://docs.aedifion.io/en/developers/kafka/
  mechanism: SASL/SCRAM-SHA-512 over SSL
  name: kafka-sasl
  note: Kafka consumers authenticate with SASL_SCRAM_SHA512 and security_protocol SSL.
  transport: kafka
  type: other
slug: aedifion-authentication
source_filename: aedifion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: searched\nsource: openapi/aedifion-openapi.yml\ndocs: https://docs.aedifion.io/en/developers/http-api/guides-and-tutorials/authentication/\ndiscovery: well-known/aedifion-openid-configuration.json\nsummary:\n  types: [http, oauth2, openIdConnect]\n  http_schemes: [basic]\n  oauth2_flows: [implicit, authorizationCode, password, clientCredentials]\n  pkce: [S256, plain]\n  mtls_client_auth: true\n  preferred: openIDConnect\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  status: legacy\n  header: 'Authorization: Basic base64(email:password)'\n  rfc: RFC 7617\n  note: >-\n    The docs state \"The aedifion HTTP API supports Basic Auth for legacy reasons until\n    further notice. HTTP Basic Auth may be deprecated in future.\" Credentials are the user's\n    platform email and password, sent on every request, so it must only be used over HTTPS.\n  sources: [openapi/aedifion-openapi.yml]\n- name: openIDConnect\n  type: oauth2\n  subtype:\
  \ openIdConnect\n  issuer: https://auth.aedifion.io/realms/aedifion\n  provider: Keycloak\n  header: 'Authorization: Bearer <access_token>'\n  endpoints:\n    authorization: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/auth\n    token: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/token\n    introspection: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/token/introspect\n    jwks_uri: https://auth.aedifion.io/realms/aedifion/protocol/openid-connect/certs\n  flows:\n  - flow: implicit\n    declared_in: openapi\n  - flow: authorizationCode\n    declared_in: oidc-discovery\n  - flow: password\n    declared_in: docs\n    note: Keycloak Direct Access Grant - grant_type=password with client_id, username, password.\n  - flow: clientCredentials\n    declared_in: oidc-discovery\n  token_endpoint_auth_methods:\n  - private_key_jwt\n  - client_secret_basic\n  - client_secret_post\n  - tls_client_auth\n  - client_secret_jwt\n  sources: [openapi/aedifion-openapi.yml,\
  \ well-known/aedifion-openid-configuration.json]\n- name: mqtt-credentials\n  type: other\n  transport: mqtt\n  note: >-\n    The MQTT broker at mqtt.aedifion.io authenticates with username/password in the MQTT\n    CONNECT packet over TLS. Limited-validity credentials are minted through the HTTP API's\n    MQTT user-management endpoints; unlimited-validity credentials are issued only on\n    request by aedifion staff. Authorization is per-topic read/write.\n  docs: https://docs.aedifion.io/en/developers/http-api/guides-and-tutorials/mqtt-user-management/\n- name: kafka-sasl\n  type: other\n  transport: kafka\n  mechanism: SASL/SCRAM-SHA-512 over SSL\n  note: Kafka consumers authenticate with SASL_SCRAM_SHA512 and security_protocol SSL.\n  docs: https://docs.aedifion.io/en/developers/kafka/\nsso:\n  supported: true\n  protocols: [OpenID Connect, OAuth 2.0, SAML, LDAP, Active Directory]\n  docs: https://docs.aedifion.io/en/admins/sso/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aedifion/refs/heads/main/authentication/aedifion-authentication.yml
summary_line: http/oauth2/openIdConnect · 4 schemes
tags:
- Building Automation
- Smart Buildings
- Energy Management
- Internet of Things
- Real Estate
- HVAC
- Sustainability
- Time Series
- Analytics
- MQTT
- Building Operations
- ESG
- PropTech
- Germany
---
