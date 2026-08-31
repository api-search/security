---
api_key_in: []
auth_types:
- oauth2
- http
- ims-enterprise
description: ''
kind: authentication
layout: security
method: searched
name: Itslearning Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: itslearning secures its APIs with oauth2, http, and ims-enterprise across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: itslearning
provider_slug: itslearning
scheme_count: 3
schemes:
- applies_to: LTI Integration
  description: LTI 1.3 Core and LTI Advantage use the IMS Security Framework — OpenID Connect third-party-initiated login plus OAuth 2.0 client_credentials with signed JWT client assertions and JWKS key sets for tool <-> platform messaging. itslearning holds LTI Advantage Complete certification.
  name: LTI 1.3 / OAuth2
  scheme: clientCredentials
  standards:
  - lti-1.3
  - lti-advantage
  - oauth2
  - oidc
  - jwt
  type: oauth2
- applies_to:
  - Organisation API
  - IMS Enterprise Services
  description: The SOAP Organisation API (DataService/ReadDataService/FileService/FileStreamService/InstanceService) and IMS Enterprise Services are authenticated per itslearning site with issued service credentials.
  name: Organisation API credentials
  type: http
- applies_to: Data Warehouse API
  description: OData Data Warehouse access is provisioned per customer via the account manager; credentials are issued to the customer's reporting/BI connection.
  name: Data Warehouse OData access
  type: http
slug: itslearning-authentication
source_filename: itslearning-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.itslearning.com/\ndocs: https://developer.itslearning.com/Content-and-tool-integrations.html\nnote: >-\n  itslearning has no OpenAPI to derive from; this profile is captured from the developer portal.\n  Different API surfaces use different auth models.\nsummary:\n  types: [oauth2, http, ims-enterprise]\n  oauth2_flows: [clientCredentials]\nschemes:\n- name: LTI 1.3 / OAuth2\n  type: oauth2\n  scheme: clientCredentials\n  description: >-\n    LTI 1.3 Core and LTI Advantage use the IMS Security Framework — OpenID Connect third-party-initiated\n    login plus OAuth 2.0 client_credentials with signed JWT client assertions and JWKS key sets for\n    tool <-> platform messaging. itslearning holds LTI Advantage Complete certification.\n  applies_to: LTI Integration\n  standards: [lti-1.3, lti-advantage, oauth2, oidc, jwt]\n- name: Organisation API credentials\n  type: http\n  description: >-\n    The SOAP Organisation\
  \ API (DataService/ReadDataService/FileService/FileStreamService/InstanceService)\n    and IMS Enterprise Services are authenticated per itslearning site with issued service credentials.\n  applies_to: [Organisation API, IMS Enterprise Services]\n- name: Data Warehouse OData access\n  type: http\n  description: >-\n    OData Data Warehouse access is provisioned per customer via the account manager; credentials are\n    issued to the customer's reporting/BI connection.\n  applies_to: Data Warehouse API\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/itslearning/refs/heads/main/authentication/itslearning-authentication.yml
summary_line: oauth2/http/ims-enterprise · 3 schemes
tags:
- Company
- Saas
- Education
- EdTech
- Learning Management System
- LMS
- LTI
- Norway
---
