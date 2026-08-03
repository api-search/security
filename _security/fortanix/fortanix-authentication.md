---
api_key_in:
- header
api_specs:
- filename: fortanix-dsm-openapi-original.json
  format: json
  label: Fortanix Data Security Manager REST API
  slug: dsm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/openapi/fortanix-dsm-openapi-original.json
- filename: fortanix-ccm-openapi-original.json
  format: json
  label: Fortanix Confidential Computing Manager REST API
  slug: ccm
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/openapi/fortanix-ccm-openapi-original.json
- filename: fortanix-armor-key-insight-openapi-original.json
  format: json
  label: Fortanix Armor and Key Insight API
  slug: armor-key-insight
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/openapi/fortanix-armor-key-insight-openapi-original.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Fortanix Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Fortanix secures its APIs with apiKey, http, and oauth2 across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Fortanix
provider_slug: fortanix
scheme_count: 5
schemes:
- description: OAuth 2.0 client credential flow, see https://datatracker.ietf.org/doc/html/rfc6749#section-4.4.
  flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://api.armor.fortanix.com/api/v1/iam/session/oauth2/token
  name: Oauth2ClientCredentials
  sources:
  - openapi/fortanix-armor-key-insight-openapi-original.json
  type: oauth2
- description: A JWT bearer token to be passed once authenticated.
  in: header
  name: bearerToken
  parameter: Authentication
  sources:
  - openapi/fortanix-ccm-openapi-original.json
  type: apiKey
- name: basicAuth
  scheme: basic
  sources:
  - openapi/fortanix-dsm-openapi-original.json
  type: http
- description: Please enter your token prefixed with 'Basic ' (e.g., 'Basic your_token_here')
  in: header
  name: apiKeyAuth
  parameter: Authorization
  sources:
  - openapi/fortanix-dsm-openapi-original.json
  type: apiKey
- bearerFormat: JWT
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/fortanix-dsm-openapi-original.json
  type: http
slug: fortanix-authentication
source_filename: fortanix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: openapi/fortanix-armor-key-insight-openapi-original.json, openapi/fortanix-ccm-openapi-original.json,\n  openapi/fortanix-dsm-openapi-original.json\ndocs:\n- name: Authentication - App and User (DSM)\n  url: https://support.fortanix.com/docs/fortanix-authentication-app-and-user\n- name: User Authentication (DSM)\n  url: https://support.fortanix.com/docs/user-authentication\n- name: Configure API Client and Client Authentication (DSM)\n  url: https://support.fortanix.com/docs/dsm-configure-api-client-and-client-authentication\n- name: Application Authentication with Client Certificate (DSM)\n  url: https://support.fortanix.com/docs/dsm-example-code-app-authentication-with-client-certificate\n- name: Programmatic Access to Fortanix Armor IAM\n  url: https://support.fortanix.com/docs/programmatic-access-to-fortanix-armor-iam\n- name: Client Credentials Flow (Key Insight)\n  url: https://support.fortanix.com/docs/fortanix-key-insight-aws-client-credentials-flow\n\
  - name: Okta Configuration For Client Credentials Authentication (Key Insight)\n  url: https://support.fortanix.com/docs/fortanix-key-insight-okta-configuration-for-client-credentials-authentication\n- name: Auth0 Configuration For Client Credentials Authentication (Key Insight)\n  url: https://support.fortanix.com/docs/fortanix-key-insight-auth0-configuration-for-client-credentials-authentication\nby_api:\n  fortanix:dsm:\n    model: session-bearer-or-direct-key\n    schemes:\n    - basicAuth\n    - apiKeyAuth\n    - bearerToken\n    detail: 'DSM accepts HTTP Basic with an app credential (app UUID + API key) or user\n      credentials, an apiKey header named Authorization carrying a token prefixed with\n      \"Basic \", or an HTTP bearer JWT minted by POST /sys/v1/session/auth (Authenticate).\n      Client-certificate authentication for applications is also supported.'\n    session_operations:\n    - AuthDiscover\n    - Authenticate\n    - SelectAccount\n    - Refresh\n    - Reauthenticate\n\
  \    - Terminate\n    mfa:\n      supported: true\n      operations:\n      - U2fAuth\n      - RecoveryCodeAuth\n      - Config2faAuth\n      - Config2faTerminate\n      - GenerateRecoveryCodes\n    federation:\n      saml: 'DSM publishes SAML SP metadata at GET /saml/metadata.xml (SamlSpMetadata).'\n      ldap: 'LDAP/AD integration via LdapSearch and TestLdapConfig, with external roles\n        mapped onto DSM groups.'\n    authorization_model: 'Authorization is group membership, not scopes. An app or user\n      may operate on a security object only if it is a member of that object''s group;\n      per-group memberships further restrict which operations are permitted.'\n  fortanix:ccm:\n    model: jwt-bearer\n    schemes:\n    - bearerToken\n    detail: 'A JWT bearer token passed once authenticated, in a header literally named\n      \"Authentication\" (not \"Authorization\") — a non-standard header name that trips\n      generic OAuth clients.'\n  fortanix:armor-key-insight:\n    model:\
  \ oauth2-client-credentials\n    schemes:\n    - Oauth2ClientCredentials\n    detail: 'OAuth 2.0 client credentials (RFC 6749 section 4.4) against https://api.armor.fortanix.com/api/v1/iam/session/oauth2/token.\n      The flow declares an EMPTY scopes map — there are no published scopes; authorization\n      rides on the credential identity. Okta and Auth0 are documented as external\n      authorization servers for this flow.'\n    session_operations:\n    - OauthToken\n    - Terminate\ndiscovery:\n  openid_configuration: false\n  oauth_authorization_server: false\n  note: 'No RFC 8414 or OIDC discovery document is served on any Fortanix host, so\n    the token endpoint is discoverable only from the OpenAPI and the docs. See well-known/fortanix-well-known.yml.'\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Oauth2ClientCredentials\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl:\
  \ https://api.armor.fortanix.com/api/v1/iam/session/oauth2/token\n    scopes: 0\n  description: OAuth 2.0 client credential flow, see https://datatracker.ietf.org/doc/html/rfc6749#section-4.4.\n  sources:\n  - openapi/fortanix-armor-key-insight-openapi-original.json\n- name: bearerToken\n  type: apiKey\n  in: header\n  parameter: Authentication\n  description: A JWT bearer token to be passed once authenticated.\n  sources:\n  - openapi/fortanix-ccm-openapi-original.json\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/fortanix-dsm-openapi-original.json\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Please enter your token prefixed with 'Basic ' (e.g., 'Basic your_token_here')\n  sources:\n  - openapi/fortanix-dsm-openapi-original.json\n- name: bearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/fortanix-dsm-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fortanix/refs/heads/main/authentication/fortanix-authentication.yml
summary_line: apiKey/http/oauth2 · 5 schemes
tags:
- Company
- Security
- Encryption
- Key Management
- Cryptography
- Confidential Computing
- HSM
- Data Security
- Post-Quantum
- Secrets Management
---
