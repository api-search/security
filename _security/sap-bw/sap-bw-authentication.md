---
api_key_in:
- header
- cookie
auth_types:
- http
- apiKey
- oauth2
- mutualTLS
description: SAP BW/4HANA has no vendor-hosted API gateway and therefore no vendor-issued credential. Authentication is whatever the customer's own SAP NetWeaver Application Server for ABAP is configured for, and every mechanism below is an AS ABAP / Internet Communication Framework capability that SAP documents for BW, not an SAP BW-specific auth scheme. Derived from SAP's published security documentation, not from an OpenAPI securitySchemes block - this repo holds no spec, because SAP publishes none for BW.
kind: authentication
layout: security
method: searched
name: Sap Bw Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- saml2Bearer
overview: SAP BW secures its APIs with http, apiKey, oauth2, and mutualTLS across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and saml2Bearer flow(s).
provider_name: SAP BW
provider_slug: sap-bw
scheme_count: 6
schemes:
- description: SAP user name and password over HTTPS against the ABAP Internet Communication Framework node that serves the OData or InA service. Documented and widely used for BW OData/ODP extraction, but SAP's own security guidance treats it as the fallback, not the target state.
  name: basic
  scheme: basic
  source: help.sap.com Authentication and Single Sign-On
  surface:
  - sap-bw:odata-api
  - sap-bw:ina-api
  type: http
- description: SAP logon ticket issued by an SAP ticket-issuing system and presented as a cookie. The classic SAP single sign-on mechanism for HTTP access to AS ABAP.
  in: cookie
  name: sap-logon-ticket
  parameter_name: MYSAPSSO2
  source: help.sap.com Authentication and Single Sign-On
  surface:
  - sap-bw:odata-api
  - sap-bw:ina-api
  type: apiKey
- description: SAML 2.0 assertion, used both for browser SSO into BW web surfaces and as a bearer assertion exchanged for an OAuth 2.0 token at the AS ABAP OAuth 2.0 authorization server. This is the mechanism behind SAP Analytics Cloud live connections to SAP BW.
  flow: saml2Bearer
  name: saml2-bearer
  source: help.sap.com Authentication and Single Sign-On
  surface:
  - sap-bw:odata-api
  - sap-bw:ina-api
  type: oauth2
- authorization_url: null
  description: AS ABAP ships an OAuth 2.0 authorization server (transaction SOAUTH2) that protects OData services published through SAP Gateway, including the BW ODP extraction service. Endpoints, clients and scopes are created per customer system - there is no SAP-hosted authorization server and therefore no discoverable /.well-known/oauth-authorization-server. Probed anyway on every SAP host in this profile; see well-known/sap-bw-well-known.yml, all misses.
  flows:
  - authorizationCode
  - clientCredentials
  - saml2Bearer
  name: oauth2
  note: Both URLs are null because they are per-installation (https://{sap-bw-host}:{port}/sap/bc/sec/oauth2/authorize and /sap/bc/sec/oauth2/token on the customer's own system). Recording a concrete URL here would assert a host SAP does not operate.
  scopes_documented: false
  surface:
  - sap-bw:odata-api
  token_url: null
  type: oauth2
- description: X.509 client certificates over HTTPS, mapped to SAP users in the ABAP system. SAP's documented option for system-to-system HTTP access.
  name: x509-client-certificate
  source: help.sap.com Authentication and Single Sign-On
  surface:
  - sap-bw:odata-api
  - sap-bw:ina-api
  type: mutualTLS
- description: Secure Network Communications - SAP's own transport-security and authentication layer for the RFC/DIAG protocols. This is what protects the BAPI/RFC surface reached through SAP JCo, PyRFC and node-rfc; RFC is not an HTTP protocol and none of the HTTP schemes above apply to it.
  name: snc
  scheme: proprietary
  source: help.sap.com Establishing Secure Network Communication
  surface:
  - sap-bw:bapi-api
  type: http
slug: sap-bw-authentication
source_filename: sap-bw-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: >-\n  https://help.sap.com/docs/SAP_BW4HANA/d3b558c9e49d4eb495c99c63a0ae549a/4f0ab13ed47c5f87e10000000a42189b.html\ndocs:\n  - name: Authentication and Single Sign-On\n    url: https://help.sap.com/docs/SAP_BW4HANA/d3b558c9e49d4eb495c99c63a0ae549a/4f0ab13ed47c5f87e10000000a42189b.html\n  - name: User Administration and Authentication\n    url: https://help.sap.com/docs/SAP_BW4HANA/d3b558c9e49d4eb495c99c63a0ae549a/4f0a05dde2a4606ee10000000a42189e.html\n  - name: Communication Channel Security\n    url: https://help.sap.com/docs/SAP_BW4HANA/d3b558c9e49d4eb495c99c63a0ae549a/4f0a063fe2a4606ee10000000a42189e.html\n  - name: Establishing Secure Network Communication (SNC)\n    url: https://help.sap.com/docs/SAP_BW4HANA/841c96bc79644fcfb9fa7103aad9c15b/fdc0a4683c5b43d1aa5c26497b3927e8.html\n  - name: Web Services and ICF Services\n    url: https://help.sap.com/docs/SAP_BW4HANA/d3b558c9e49d4eb495c99c63a0ae549a/b31dd13ffc9a4a21e10000000a1550b0.html\n\
  description: >-\n  SAP BW/4HANA has no vendor-hosted API gateway and therefore no vendor-issued\n  credential. Authentication is whatever the customer's own SAP NetWeaver\n  Application Server for ABAP is configured for, and every mechanism below is\n  an AS ABAP / Internet Communication Framework capability that SAP documents\n  for BW, not an SAP BW-specific auth scheme. Derived from SAP's published\n  security documentation, not from an OpenAPI securitySchemes block - this\n  repo holds no spec, because SAP publishes none for BW.\nsummary:\n  types: [http, apiKey, oauth2, mutualTLS]\n  vendor_issued_credentials: false\n  per_customer_configured: true\n  api_key_in: [header, cookie]\n  oauth2_flows: [authorizationCode, clientCredentials, saml2Bearer]\nschemes:\n  - name: basic\n    type: http\n    scheme: basic\n    surface: [sap-bw:odata-api, sap-bw:ina-api]\n    description: >-\n      SAP user name and password over HTTPS against the ABAP Internet\n      Communication Framework node\
  \ that serves the OData or InA service.\n      Documented and widely used for BW OData/ODP extraction, but SAP's own\n      security guidance treats it as the fallback, not the target state.\n    source: help.sap.com Authentication and Single Sign-On\n  - name: sap-logon-ticket\n    type: apiKey\n    in: cookie\n    parameter_name: MYSAPSSO2\n    surface: [sap-bw:odata-api, sap-bw:ina-api]\n    description: >-\n      SAP logon ticket issued by an SAP ticket-issuing system and presented as\n      a cookie. The classic SAP single sign-on mechanism for HTTP access to\n      AS ABAP.\n    source: help.sap.com Authentication and Single Sign-On\n  - name: saml2-bearer\n    type: oauth2\n    flow: saml2Bearer\n    surface: [sap-bw:odata-api, sap-bw:ina-api]\n    description: >-\n      SAML 2.0 assertion, used both for browser SSO into BW web surfaces and\n      as a bearer assertion exchanged for an OAuth 2.0 token at the AS ABAP\n      OAuth 2.0 authorization server. This is the mechanism behind\
  \ SAP\n      Analytics Cloud live connections to SAP BW.\n    source: help.sap.com Authentication and Single Sign-On\n  - name: oauth2\n    type: oauth2\n    flows: [authorizationCode, clientCredentials, saml2Bearer]\n    surface: [sap-bw:odata-api]\n    description: >-\n      AS ABAP ships an OAuth 2.0 authorization server (transaction SOAUTH2)\n      that protects OData services published through SAP Gateway, including\n      the BW ODP extraction service. Endpoints, clients and scopes are\n      created per customer system - there is no SAP-hosted authorization\n      server and therefore no discoverable\n      /.well-known/oauth-authorization-server. Probed anyway on every SAP host\n      in this profile; see well-known/sap-bw-well-known.yml, all misses.\n    scopes_documented: false\n    authorization_url: null\n    token_url: null\n    note: >-\n      Both URLs are null because they are per-installation\n      (https://{sap-bw-host}:{port}/sap/bc/sec/oauth2/authorize and\n      /sap/bc/sec/oauth2/token\
  \ on the customer's own system). Recording a\n      concrete URL here would assert a host SAP does not operate.\n  - name: x509-client-certificate\n    type: mutualTLS\n    surface: [sap-bw:odata-api, sap-bw:ina-api]\n    description: >-\n      X.509 client certificates over HTTPS, mapped to SAP users in the ABAP\n      system. SAP's documented option for system-to-system HTTP access.\n    source: help.sap.com Authentication and Single Sign-On\n  - name: snc\n    type: http\n    scheme: proprietary\n    surface: [sap-bw:bapi-api]\n    description: >-\n      Secure Network Communications - SAP's own transport-security and\n      authentication layer for the RFC/DIAG protocols. This is what protects\n      the BAPI/RFC surface reached through SAP JCo, PyRFC and node-rfc;\n      RFC is not an HTTP protocol and none of the HTTP schemes above apply\n      to it.\n    source: help.sap.com Establishing Secure Network Communication\nauthorization:\n  model: SAP analysis authorizations + ABAP authorization\
  \ objects\n  description: >-\n    Data-level access in SAP BW is governed by analysis authorizations\n    (transaction RSECADMIN) layered on top of standard ABAP authorization\n    objects - not by API scopes. An OAuth scope, where OAuth is used at all,\n    grants access to an OData service; what rows come back is decided by the\n    calling user's analysis authorizations.\n  docs: https://help.sap.com/docs/SAP_BW4HANA/107a6e8a38b74ede94c833ca3b7b6f51/4cbb3bdbf7ec4195909005e875e6bb51.html\nscopes_artifact: null\nscopes_note: >-\n  scopes/ is deliberately absent. OAuth scopes in AS ABAP are created per\n  customer system against locally published OData services; SAP publishes no\n  scope reference for SAP BW, and deriving one would mean inventing scope\n  names for services that do not exist until a customer generates them.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sap-bw/refs/heads/main/authentication/sap-bw-authentication.yml
summary_line: http/apiKey/oauth2/mutualTLS · 6 schemes
tags:
- Business Intelligence
- Data Warehousing
- Enterprise
- ETL
- SAP
---
