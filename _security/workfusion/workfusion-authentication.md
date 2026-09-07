---
anonymous_access: false
api_key_in:
- cookie
- header
auth_types:
- http
- apiKey
- mutualTLS
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 5
method: searched
name: Workfusion Authentication
name_suffix: Authentication
oauth_flows: []
overview: WorkFusion secures its APIs with http, apiKey, mutualTLS, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: WorkFusion
provider_slug: workfusion
scheme_count: 5
schemes:
- description: Primary mechanism. POST /workfusion/api/dologin with Content-Type application/x-www-form-urlencoded and the fields j_username and j_password (Control Tower credentials). The response body is {"success":true,"csrfToken":..., "csrfHeaderName":...} and the Set-Cookie response header carries JSESSIONID. Every subsequent request sends the JSESSIONID cookie.
  in: cookie
  name: FormLoginSession
  parameter: JSESSIONID
  sources:
  - https://doc.workfusion.com/platform/docs/api/workfusion-rest-api
  type: apiKey
- description: CSRF protection is applied to the REST endpoints. The csrfToken value returned by /dologin must be echoed on every subsequent call in the header named by csrfHeaderName (X-CSRF-TOKEN in the provider's own samples).
  in: header
  name: CsrfToken
  parameter: X-CSRF-TOKEN
  sources:
  - https://doc.workfusion.com/platform/docs/api/workfusion-rest-api
  type: apiKey
- description: 'The Packages API (/mturk-web/soap/api) is documented with `Authorization: Basic` and curl --user user:password rather than the form-login session.'
  name: HttpBasic
  scheme: basic
  sources:
  - https://doc.workfusion.com/platform/docs/api/packages-api
  type: http
- description: Optional client-certificate authentication. A PKCS#12 client certificate is issued per username and imported to the caller; Tomcat is configured with clientAuth=true on an SSL connector and the JNDI variable rest/cert-auth/enable set to true. This is a deployment-time option the customer enables, not a hosted default.
  name: CertificateBasedAuthentication
  sources:
  - https://doc.workfusion.com/platform/docs/api/certificate-based-authentication
  type: mutualTLS
- description: From IA Cloud 10.2 the platform federates identity through Keycloak (SAML/OIDC IdPs, LDAP). REST callers authenticate with Keycloak credentials, but the provider documents that a LOCAL password must be set in Keycloak for the user because an IdP-issued password is never held by Keycloak — i.e. REST access still resolves to a username/password login, not to a bearer token issued by the IdP. No token endpoint, no scopes and no client-credentials flow are documented for the platform API.
  name: KeycloakIdentityProvider
  sources:
  - https://doc.workfusion.com/platform/docs/install/keycloak/keycloak-and-rest-api
  - https://doc.workfusion.com/platform/docs/api/workfusion-rest-api
  type: openIdConnect
slug: workfusion-authentication
source_filename: workfusion-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: https://doc.workfusion.com/platform/docs/api/workfusion-rest-api\ndocs: https://doc.workfusion.com/platform/docs/api/workfusion-rest-api\nnote: >-\n  Derived mechanically from OpenAPI is not possible — WorkFusion publishes no OpenAPI\n  document (see conformance/ and the repo README). Every scheme below is read from the\n  provider's own public documentation on doc.workfusion.com.\nsummary:\n  types: [http, apiKey, mutualTLS, openIdConnect]\n  api_key_in: [cookie, header]\n  oauth2_flows: []\n  primary: form-login-session\nschemes:\n- name: FormLoginSession\n  type: apiKey\n  in: cookie\n  parameter: JSESSIONID\n  description: >-\n    Primary mechanism. POST /workfusion/api/dologin with Content-Type\n    application/x-www-form-urlencoded and the fields j_username and j_password (Control\n    Tower credentials). The response body is {\"success\":true,\"csrfToken\":...,\n    \"csrfHeaderName\":...} and the Set-Cookie response\
  \ header carries JSESSIONID. Every\n    subsequent request sends the JSESSIONID cookie.\n  sources: [https://doc.workfusion.com/platform/docs/api/workfusion-rest-api]\n- name: CsrfToken\n  type: apiKey\n  in: header\n  parameter: X-CSRF-TOKEN\n  description: >-\n    CSRF protection is applied to the REST endpoints. The csrfToken value returned by\n    /dologin must be echoed on every subsequent call in the header named by\n    csrfHeaderName (X-CSRF-TOKEN in the provider's own samples).\n  sources: [https://doc.workfusion.com/platform/docs/api/workfusion-rest-api]\n- name: HttpBasic\n  type: http\n  scheme: basic\n  description: >-\n    The Packages API (/mturk-web/soap/api) is documented with `Authorization: Basic`\n    and curl --user user:password rather than the form-login session.\n  sources: [https://doc.workfusion.com/platform/docs/api/packages-api]\n- name: CertificateBasedAuthentication\n  type: mutualTLS\n  description: >-\n    Optional client-certificate authentication. A PKCS#12\
  \ client certificate is issued\n    per username and imported to the caller; Tomcat is configured with clientAuth=true\n    on an SSL connector and the JNDI variable rest/cert-auth/enable set to true. This is\n    a deployment-time option the customer enables, not a hosted default.\n  sources: [https://doc.workfusion.com/platform/docs/api/certificate-based-authentication]\n- name: KeycloakIdentityProvider\n  type: openIdConnect\n  description: >-\n    From IA Cloud 10.2 the platform federates identity through Keycloak (SAML/OIDC IdPs,\n    LDAP). REST callers authenticate with Keycloak credentials, but the provider documents\n    that a LOCAL password must be set in Keycloak for the user because an IdP-issued\n    password is never held by Keycloak — i.e. REST access still resolves to a\n    username/password login, not to a bearer token issued by the IdP. No token endpoint,\n    no scopes and no client-credentials flow are documented for the platform API.\n  sources:\n  - https://doc.workfusion.com/platform/docs/install/keycloak/keycloak-and-rest-api\n\
  \  - https://doc.workfusion.com/platform/docs/api/workfusion-rest-api\ngaps:\n- no bearer/API-key credential is issued for the REST API; callers use interactive user credentials\n- no OAuth 2.0 scopes are published, so scopes/ is intentionally absent from this repo\n- no documented token rotation, expiry or revocation policy for the JSESSIONID session\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workfusion/refs/heads/main/authentication/workfusion-authentication.yml
summary_line: http/apiKey/mutualTLS/openIdConnect · 5 schemes
tags:
- AI Agents
- Financial Crime Compliance
- Anti-Money Laundering
- Sanctions Screening
- Know Your Customer
- Transaction Monitoring
- Adverse Media Monitoring
- Intelligent Document Processing
- Robotic Process Automation
- Banking
---
