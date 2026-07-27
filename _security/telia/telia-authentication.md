---
api_key_in: []
api_specs:
- filename: telia-lso-sonata-site-management.yml
  format: yaml
  label: Telia LSO Sonata Geographic Site Management API
  slug: telia-lso-sonata-geographic-site-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telia/refs/heads/main/openapi/telia-lso-sonata-site-management.yml
auth_types:
- oauth2
- http-basic
- mutualTLS
- openIdConnect
- ip-allowlist
- smpp-bind
description: ''
kind: authentication
layout: security
method: searched
name: Telia Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Telia Company secures its APIs with oauth2, http-basic, mutualTLS, openIdConnect, ip-allowlist, and smpp-bind across 8 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Telia Company
provider_slug: telia
scheme_count: 8
schemes:
- description: Token endpoint for the production environment
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api-garden.teliacompany.com/v4/oauth/client_credential/accesstoken
  name: prodBearerAuth
  sources:
  - openapi/telia-lso-sonata-site-management.yml
  surface: LSO Sonata Geographic Site Management (production)
  type: oauth2
- description: Token endpoint for all test environments
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api-garden-test.teliacompany.com/v4/oauth/client_credential/accesstoken
  name: testBearerAuth
  sources:
  - openapi/telia-lso-sonata-site-management.yml
  surface: LSO Sonata Geographic Site Management (test and sandbox)
  type: oauth2
- base_url: https://api.messaging.teliacompany.com/sms/rest/v2
  credential_source: created by a user with the Technical role in the Bulk Messaging web portal, under Services -> Technical Configuration
  evidence: public implementation guide, cURL example with an Authorization Basic header
  name: bulkMessagingBasic
  probe: https://api.messaging.teliacompany.com/sms/rest/v2/* returns HTTP 401 to an anonymous caller, confirming the challenge is live
  scheme: basic
  sources:
  - https://cdn.messaging.teliacompany.com/documents/developer/index.html
  surface: Bulk Messaging SMS REST API
  type: http
- credential_source: callback address and callback credentials are registered by the customer in the Bulk Messaging portal
  direction: inbound to the customer
  name: bulkMessagingCallbackBasic
  scheme: basic
  sources:
  - https://cdn.messaging.teliacompany.com/documents/developer/index.html
  surface: Bulk Messaging SMS Callback API (customer-implemented)
  type: http
- additional_control: static source IP addresses must be whitelisted in Telia's ACL by the Bulk Messaging Support team
  endpoint: smpp.messaging.teliacompany.com:3550
  fields:
  - system_id (username)
  - password
  interface_version: '0x34'
  name: smppBind
  sources:
  - https://cdn.messaging.teliacompany.com/documents/developer/index.html
  surface: Bulk Messaging SMPP API
  transport_security: TLS 1.2 minimum, SNI required, fixed cipher list
  type: smpp-bind
- description: Telia connects outbound to a customer-implemented receiver and authenticates with client certificates
  name: aceAudioStreamMtls
  sources:
  - https://github.com/telia-oss/ace-audio-stream-forwarding-api
  surface: Telia ACE Audio Stream Forwarding (gRPC)
  type: mutualTLS
- ciba: false
  ciba_note: no backchannel_authentication_endpoint is advertised; CIBA is the grant CAMARA specifies for network-based authorization, so no CIBA-capable authorization server is publicly discoverable on Telia's estate
  discovery_document: well-known/telia-openid-configuration.json
  endpoints:
    authorization: https://tunnistus.telia.fi/uas/oauth2/authorization
    introspection: https://tunnistus.telia.fi/uas/oauth2/introspection
    jwks: https://tunnistus.telia.fi/uas/oauth2/metadata.jwks
    revocation: https://tunnistus.telia.fi/uas/oauth2/revocation
    token: https://tunnistus.telia.fi/uas/oauth2/token
    userinfo: https://tunnistus.telia.fi/uas/oauth2/userinfo
  grant_types:
  - authorization_code
  - password
  - client_credentials
  - refresh_token
  - urn:ietf:params:oauth:grant-type:saml2-bearer
  - http://globalsign.com/iam/sso/oauth2/grant-type/sms-mt-otp
  - http://globalsign.com/iam/sso/oauth2/grant-type/smtp-otp
  id_token_signing_alg:
  - RS256
  - HS256
  issuer: https://tunnistus.telia.fi/uas
  name: tunnistusOidc
  openIdConnectUrl: https://tunnistus.telia.fi/.well-known/openid-configuration
  scopes:
  - openid
  - userinfo
  sources:
  - https://tunnistus.telia.fi/.well-known/openid-configuration
  surface: Telia Tunnistus identification broker (Telia Finland)
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
- algorithm: HMAC SHA256 (JWT)
  claims:
  - iss
  - aud
  - exp
  - iat
  - content_hash
  - method
  - path
  header: X-ACE-Signature
  name: aceKnowledgeWebhookSignature
  note: enabled per contact method by the editor, with a shared secret; Telia recommends a secret of at least 32 characters
  optional: true
  sources:
  - https://github.com/telia-oss/ace-knowledge-docs/blob/master/REST/webhook.md
  surface: ACE Knowledge contact-method webhook (outbound to the customer)
  type: request-signing
slug: telia-authentication
source_filename: telia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/telia-lso-sonata-site-management.yml\ndocs:\n- https://cdn.messaging.teliacompany.com/documents/developer/index.html\n- https://tunnistus.telia.fi/.well-known/openid-configuration\n- https://github.com/telia-oss/ace-audio-stream-forwarding-api\n- https://github.com/telia-oss/ace-knowledge-docs/blob/master/REST/webhook.md\nnotes: >-\n  Upgraded from the derived OpenAPI-only profile. Telia runs five different\n  authentication models across seven surfaces, and only one of them (oauth2\n  client credentials on LSO Sonata) is expressed in a machine-readable contract.\n  Every model below is documented on a public Telia surface.\nsummary:\n  types:\n  - oauth2\n  - http-basic\n  - mutualTLS\n  - openIdConnect\n  - ip-allowlist\n  - smpp-bind\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  scopes_published: false\n  self_serve_credentials: false\nschemes:\n- name: prodBearerAuth\n  type: oauth2\n  surface: LSO\
  \ Sonata Geographic Site Management (production)\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-garden.teliacompany.com/v4/oauth/client_credential/accesstoken\n    scopes: 0\n  description: Token endpoint for the production environment\n  sources:\n  - openapi/telia-lso-sonata-site-management.yml\n- name: testBearerAuth\n  type: oauth2\n  surface: LSO Sonata Geographic Site Management (test and sandbox)\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api-garden-test.teliacompany.com/v4/oauth/client_credential/accesstoken\n    scopes: 0\n  description: Token endpoint for all test environments\n  sources:\n  - openapi/telia-lso-sonata-site-management.yml\n- name: bulkMessagingBasic\n  type: http\n  scheme: basic\n  surface: Bulk Messaging SMS REST API\n  base_url: https://api.messaging.teliacompany.com/sms/rest/v2\n  credential_source: created by a user with the Technical role in the Bulk Messaging\n    web portal, under Services -> Technical Configuration\n\
  \  evidence: public implementation guide, cURL example with an Authorization Basic\n    header\n  probe: https://api.messaging.teliacompany.com/sms/rest/v2/* returns HTTP 401 to\n    an anonymous caller, confirming the challenge is live\n  sources:\n  - https://cdn.messaging.teliacompany.com/documents/developer/index.html\n- name: bulkMessagingCallbackBasic\n  type: http\n  scheme: basic\n  surface: Bulk Messaging SMS Callback API (customer-implemented)\n  direction: inbound to the customer\n  credential_source: callback address and callback credentials are registered by\n    the customer in the Bulk Messaging portal\n  sources:\n  - https://cdn.messaging.teliacompany.com/documents/developer/index.html\n- name: smppBind\n  type: smpp-bind\n  surface: Bulk Messaging SMPP API\n  endpoint: smpp.messaging.teliacompany.com:3550\n  fields:\n  - system_id (username)\n  - password\n  interface_version: '0x34'\n  transport_security: TLS 1.2 minimum, SNI required, fixed cipher list\n  additional_control:\
  \ static source IP addresses must be whitelisted in Telia's ACL\n    by the Bulk Messaging Support team\n  sources:\n  - https://cdn.messaging.teliacompany.com/documents/developer/index.html\n- name: aceAudioStreamMtls\n  type: mutualTLS\n  surface: Telia ACE Audio Stream Forwarding (gRPC)\n  description: Telia connects outbound to a customer-implemented receiver and\n    authenticates with client certificates\n  sources:\n  - https://github.com/telia-oss/ace-audio-stream-forwarding-api\n- name: tunnistusOidc\n  type: openIdConnect\n  surface: Telia Tunnistus identification broker (Telia Finland)\n  issuer: https://tunnistus.telia.fi/uas\n  openIdConnectUrl: https://tunnistus.telia.fi/.well-known/openid-configuration\n  discovery_document: well-known/telia-openid-configuration.json\n  endpoints:\n    authorization: https://tunnistus.telia.fi/uas/oauth2/authorization\n    token: https://tunnistus.telia.fi/uas/oauth2/token\n    userinfo: https://tunnistus.telia.fi/uas/oauth2/userinfo\n \
  \   jwks: https://tunnistus.telia.fi/uas/oauth2/metadata.jwks\n    introspection: https://tunnistus.telia.fi/uas/oauth2/introspection\n    revocation: https://tunnistus.telia.fi/uas/oauth2/revocation\n  grant_types:\n  - authorization_code\n  - password\n  - client_credentials\n  - refresh_token\n  - urn:ietf:params:oauth:grant-type:saml2-bearer\n  - http://globalsign.com/iam/sso/oauth2/grant-type/sms-mt-otp\n  - http://globalsign.com/iam/sso/oauth2/grant-type/smtp-otp\n  scopes:\n  - openid\n  - userinfo\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - client_secret_jwt\n  - private_key_jwt\n  - none\n  id_token_signing_alg:\n  - RS256\n  - HS256\n  ciba: false\n  ciba_note: no backchannel_authentication_endpoint is advertised; CIBA is the\n    grant CAMARA specifies for network-based authorization, so no CIBA-capable\n    authorization server is publicly discoverable on Telia's estate\n  sources:\n  - https://tunnistus.telia.fi/.well-known/openid-configuration\n\
  - name: aceKnowledgeWebhookSignature\n  type: request-signing\n  surface: ACE Knowledge contact-method webhook (outbound to the customer)\n  header: X-ACE-Signature\n  algorithm: HMAC SHA256 (JWT)\n  claims:\n  - iss\n  - aud\n  - exp\n  - iat\n  - content_hash\n  - method\n  - path\n  optional: true\n  note: enabled per contact method by the editor, with a shared secret; Telia\n    recommends a secret of at least 32 characters\n  sources:\n  - https://github.com/telia-oss/ace-knowledge-docs/blob/master/REST/webhook.md\nonboarding:\n  self_serve: false\n  requirements:\n  - an existing Telia commercial agreement\n  - a whitelisted corporate email domain\n  - manual support approval of the developer account\n  - a second approval of the registered application\n  - a separate fee agreement per API (Telia Developer's Toolbox terms of use)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telia/refs/heads/main/authentication/telia-authentication.yml
summary_line: oauth2/http-basic/mutualTLS/openIdConnect/ip-allowlist/smpp-bind · 8 schemes
tags:
- Telecommunications
- Sweden
- Nordics
- Baltics
- Mobile Network Operator
- Network APIs
- CAMARA
- Open Gateway
- Messaging
- SMS
- SMPP
- IoT
- 5G
- Broadband
- Identity Verification
- BSS
- OSS
- TM Forum
- MEF
- Standards
---
