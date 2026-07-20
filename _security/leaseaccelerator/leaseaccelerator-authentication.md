---
api_key_in: []
api_specs:
- filename: leaseaccelerator-api-openapi.yml
  format: yaml
  label: LeaseAccelerator API
  slug: leaseaccelerator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/leaseaccelerator/refs/heads/main/openapi/leaseaccelerator-api-openapi.yml
auth_types:
- saml2
- session-token
description: 'How a client authenticates to the LeaseAccelerator API. LeaseAccelerator does not issue API keys or OAuth tokens. Access is secured by SAML2 against the customer''s own identity provider: the client performs a SAML2 ECP exchange with the LeaseAccelerator service provider endpoint, receives a text security token, and submits that token as a form field on every subsequent API POST.'
kind: authentication
layout: security
method: searched
name: Leaseaccelerator Authentication
name_suffix: Authentication
oauth_flows: []
overview: LeaseAccelerator secures its APIs with saml2 and session-token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LeaseAccelerator
provider_slug: leaseaccelerator
scheme_count: 1
schemes:
- description: A text security token obtained from the LeaseAccelerator SAML2 authentication layer. Instantiates a secure session that can be used for multiple, concurrent, stateless method requests.
  flow:
  - action: Obtain the URL for your identity provider (IdP) and login credentials for a user already federated for access in LeaseAccelerator.
    step: 1
  - action: Submit a SAML2 GET request to the LeaseAccelerator service provider (SP) URL https://{environment}.leaseaccelerator.com/auth/api, identifying the IdP and the credentials to use. This requires an identity provider that supports Enhanced Client or Proxy (ECP) mode.
    step: 2
  - action: Extract the response, which takes the form of a text security token.
    step: 3
  - action: POST to https://{environment}.leaseaccelerator.com/lease_accelerator/api/LeaseAccelerator/{operation} with the `token` field set to that security token and the `file` field set to the <APIRequest> document.
    step: 4
  name: saml2Token
  reference_implementation:
    first_party: false
    language: java
    library: shib-http-client
    note: The LeaseAccelerator developer documentation recommends this library for Java clients and publishes a complete Java test client as an appendix, using the IdP endpoint {idpBaseUrl}/idp/profile/SAML2/SOAP/ECP.
    url: https://github.com/DARIAH-DE/shib-http-client
  standards:
  - SAML 2.0 (OASIS)
  - SAML 2.0 Enhanced Client or Proxy (ECP) profile
  token_endpoint: https://{environment}.leaseaccelerator.com/auth/api
  token_endpoint_production: https://www.leaseaccelerator.com/auth/api
  transport: multipart/form-data field `token` on the operation POST
  type: saml2-bearer-token
slug: leaseaccelerator-authentication
source_filename: leaseaccelerator-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://docs-leaseaccelerator.insightsoftware.com/hc/en-us/articles/33895814655245-Application-Programming-Interface-API-for-Developers\ndescription: >-\n  How a client authenticates to the LeaseAccelerator API. LeaseAccelerator does not issue API keys or\n  OAuth tokens. Access is secured by SAML2 against the customer's own identity provider: the client\n  performs a SAML2 ECP exchange with the LeaseAccelerator service provider endpoint, receives a text\n  security token, and submits that token as a form field on every subsequent API POST.\nsummary:\n  types:\n  - saml2\n  - session-token\n  api_keys: false\n  oauth2: false\n  oidc: false\n  mtls: false\n  prerequisite: >-\n    The customer must be integrated with LeaseAccelerator's Single Sign-On (SSO) solution, which is\n    generally a matter of exchanging SAML2 Metadata (certificate and configuration information) with a\n    SAML2-compliant identity provider.\nschemes:\n\
  - name: saml2Token\n  type: saml2-bearer-token\n  transport: multipart/form-data field `token` on the operation POST\n  description: >-\n    A text security token obtained from the LeaseAccelerator SAML2 authentication layer. Instantiates a\n    secure session that can be used for multiple, concurrent, stateless method requests.\n  token_endpoint: https://{environment}.leaseaccelerator.com/auth/api\n  token_endpoint_production: https://www.leaseaccelerator.com/auth/api\n  flow:\n  - step: 1\n    action: >-\n      Obtain the URL for your identity provider (IdP) and login credentials for a user already federated\n      for access in LeaseAccelerator.\n  - step: 2\n    action: >-\n      Submit a SAML2 GET request to the LeaseAccelerator service provider (SP) URL\n      https://{environment}.leaseaccelerator.com/auth/api, identifying the IdP and the credentials to use.\n      This requires an identity provider that supports Enhanced Client or Proxy (ECP) mode.\n  - step: 3\n    action: Extract\
  \ the response, which takes the form of a text security token.\n  - step: 4\n    action: >-\n      POST to https://{environment}.leaseaccelerator.com/lease_accelerator/api/LeaseAccelerator/{operation}\n      with the `token` field set to that security token and the `file` field set to the <APIRequest>\n      document.\n  standards:\n  - SAML 2.0 (OASIS)\n  - SAML 2.0 Enhanced Client or Proxy (ECP) profile\n  reference_implementation:\n    language: java\n    library: shib-http-client\n    url: https://github.com/DARIAH-DE/shib-http-client\n    note: >-\n      The LeaseAccelerator developer documentation recommends this library for Java clients and publishes\n      a complete Java test client as an appendix, using the IdP endpoint\n      {idpBaseUrl}/idp/profile/SAML2/SOAP/ECP.\n    first_party: false\ntransport_security:\n  protocol: HTTPS\n  note: >-\n    LeaseAccelerator's API uses industry standard HTTPS (secure hypertext transfer protocol) with SAML 2\n    authentication for data transfer.\n\
  \  detail: security/leaseaccelerator-domain-security.yml\nuser_provisioning:\n  note: >-\n    LeaseAccelerator exposes SSO user lifecycle management as API operations rather than a separate SCIM\n    endpoint. These operations are intended for use only in environments where Single Sign-On is in use.\n  operations:\n  - FederateUser\n  - UpdateUser\n  - RevokeUser\nscopes:\n  model: role-and-scope-of-access\n  note: >-\n    Authorization is not expressed as OAuth scopes. Access is governed by LeaseAccelerator Access Control\n    roles and a ScopeOfAccess assigned to the federated user (set via the UpdateUser and FederateUser\n    operations). Because there is no OAuth surface, this repo carries no scopes/ artifact.\ndocs: https://docs-leaseaccelerator.insightsoftware.com/hc/en-us/articles/33895814655245-Application-Programming-Interface-API-for-Developers\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/leaseaccelerator/refs/heads/main/authentication/leaseaccelerator-authentication.yml
summary_line: saml2/session-token · 1 scheme
tags:
- Company
- Lease Accounting
- Lease Administration
- Financial Reporting
- Enterprise Software
- Accounting
- Real Estate
- Asset Management
- ERP Integration
- Compliance
---
