---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Rhapsody Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Rhapsody secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Rhapsody
provider_slug: rhapsody
scheme_count: 2
schemes:
- authorizationUrl: https://lyniate-docs.auth.us-east-1.amazoncognito.com/oauth2/authorize
  evidence: 307 redirect from docs host to Cognito /oauth2/authorize with response_type=code
  flow: authorizationCode
  name: docs-portal-sso
  pkce: S256
  provider: AWS Cognito (user pool "lyniate-docs", us-east-1)
  scopes:
  - openid
  - email
  - profile
  surface: Developer documentation portal (docs.rhapsody.health)
  type: oauth2
- access: Existing Rhapsody / Corepoint customers only
  evidence: Axon solution page states access via OneLogin for existing customers
  name: axon-agent-sso
  provider: OneLogin
  surface: Rhapsody Axon AI agent (chat.axon.rhapsody.health)
  type: openIdConnect
slug: rhapsody-authentication
source_filename: rhapsody-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: searched\nsource: >-\n  Observed 307 redirect from https://docs.rhapsody.health/ to the AWS Cognito\n  hosted UI (lyniate-docs.auth.us-east-1.amazoncognito.com/oauth2/authorize);\n  https://rhapsody.health/solutions/rhapsody-axon/ ;\n  https://rhapsody.health/solutions/guardian/\nnote: >-\n  Rhapsody's product REST/administration and FHIR API reference is gated behind\n  docs.rhapsody.health, so the product APIs' own security schemes are not\n  publicly observable and are NOT asserted here (no public OpenAPI to derive\n  from). What IS observable is the authentication fronting the developer surface:\n  the documentation portal and the Axon agent both sit behind enterprise SSO.\n  This profile records that observed surface honestly; it is not a claim about\n  the product API token model.\nsummary:\n  types: [oauth2, openIdConnect]\n  oauth2_flows: [authorizationCode]\n  gated: true\nschemes:\n- name: docs-portal-sso\n  surface: Developer documentation\
  \ portal (docs.rhapsody.health)\n  type: oauth2\n  flow: authorizationCode\n  pkce: S256\n  provider: AWS Cognito (user pool \"lyniate-docs\", us-east-1)\n  authorizationUrl: https://lyniate-docs.auth.us-east-1.amazoncognito.com/oauth2/authorize\n  scopes: [openid, email, profile]\n  evidence: 307 redirect from docs host to Cognito /oauth2/authorize with response_type=code\n- name: axon-agent-sso\n  surface: Rhapsody Axon AI agent (chat.axon.rhapsody.health)\n  type: openIdConnect\n  provider: OneLogin\n  access: Existing Rhapsody / Corepoint customers only\n  evidence: Axon solution page states access via OneLogin for existing customers\ngateway_supported_schemes:\n  product: Rhapsody Guardian\n  url: https://rhapsody.health/solutions/guardian/\n  note: >-\n    These are the authentication protocols Rhapsody's healthcare API gateway\n    supports for the APIs a CUSTOMER publishes through it — quoted from the\n    Guardian product page (\"Guardian supports OAuth 2.0, SMART on FHIR, and\
  \ Basic\n    Auth\"). They describe what the product can enforce, not the token model of a\n    Rhapsody-operated public endpoint, which remains gated.\n  schemes:\n  - oauth2\n  - smart-on-fhir\n  - http-basic\nproduct_api_auth:\n  status: gated\n  detail: >-\n    Rhapsody and Corepoint expose REST administration APIs (Corepoint 7.5.3\n    Administration REST API) and FHIR APIs whose authentication is documented in\n    the gated developer portal; not verifiable from a public specification.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rhapsody/refs/heads/main/authentication/rhapsody-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Healthcare
- United States
- Interoperability
- Integration Engine
- FHIR
- HL7
- EMPI
- Terminology
- Health Data
- MCP
- API Gateway
---
