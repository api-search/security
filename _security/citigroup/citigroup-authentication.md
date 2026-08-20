---
api_key_in: []
auth_types:
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Citigroup Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Citigroup secures its APIs with oauth2 and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Citigroup
provider_slug: citigroup
scheme_count: 3
schemes:
- consent: true
  flows:
  - flow: authorizationCode
    note: Third-party application redirects the customer to Citi to authenticate and grant consent; Citi returns an authorization code exchanged for access and refresh tokens. Consent is scoped per product family (Accounts, Money Movement, Customers, etc.).
  name: CitiOAuth2AuthorizationCode
  sca: true
  sources:
  - apis.yml (citi-authorize-api, citi-accounts-transactions-api)
  surface: Citi Developer Hub (retail open banking)
  type: oauth2
- flows:
  - flow: clientCredentials
    note: Machine-to-machine access for onboarded corporate clients; documented as OAuth 2.0 in the CitiConnect API portal.
  name: CitiConnectOAuth2
  sources:
  - apis.yml (citiconnect-api, citiconnect-worldlink-api, citiconnect-fx-api)
  surface: CitiConnect (corporate Treasury and Trade Solutions)
  type: oauth2
- name: CitiConnectMutualTLS
  note: Client-certificate (mutual TLS) is required in addition to OAuth 2.0 for CitiConnect enterprise connectivity, per Citi's published CitiConnect documentation.
  sources:
  - apis.yml (citiconnect-api)
  surface: CitiConnect (corporate Treasury and Trade Solutions)
  type: mutualTLS
slug: citigroup-authentication
source_filename: citigroup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: >-\n  Citi Developer Hub / Citi Partner Portal and CitiConnect API documentation\n  (partner.citi.com/developers, developer.citi.com, citigroup.com CitiConnect\n  API portal). No public OpenAPI is published, so securitySchemes are\n  transcribed from Citi's published HTML documentation rather than derived\n  from a machine-readable spec.\ndocs:\n  - https://partner.citi.com/developers\n  - https://www.citigroup.com/global/insights/citiconnect-api-portal\nsummary:\n  types:\n    - oauth2\n    - mutualTLS\n  api_key_in: []\n  oauth2_flows:\n    - authorizationCode\n    - clientCredentials\n  notes: >-\n    Two distinct authentication surfaces. The retail Citi Developer Hub uses\n    OAuth 2.0 authorization-code with an explicit customer consent (strong\n    customer authentication) step to authorize third-party access to a\n    consenting customer's account data and payment initiation. The corporate\n    CitiConnect (Treasury\
  \ and Trade Solutions) channel uses OAuth 2.0 together\n    with mutual TLS (client-certificate) for enterprise ERP/TMS connectivity.\nschemes:\n  - name: CitiOAuth2AuthorizationCode\n    type: oauth2\n    surface: Citi Developer Hub (retail open banking)\n    flows:\n      - flow: authorizationCode\n        note: >-\n          Third-party application redirects the customer to Citi to\n          authenticate and grant consent; Citi returns an authorization code\n          exchanged for access and refresh tokens. Consent is scoped per\n          product family (Accounts, Money Movement, Customers, etc.).\n    consent: true\n    sca: true\n    sources:\n      - apis.yml (citi-authorize-api, citi-accounts-transactions-api)\n  - name: CitiConnectOAuth2\n    type: oauth2\n    surface: CitiConnect (corporate Treasury and Trade Solutions)\n    flows:\n      - flow: clientCredentials\n        note: >-\n          Machine-to-machine access for onboarded corporate clients; documented\n          as\
  \ OAuth 2.0 in the CitiConnect API portal.\n    sources:\n      - apis.yml (citiconnect-api, citiconnect-worldlink-api, citiconnect-fx-api)\n  - name: CitiConnectMutualTLS\n    type: mutualTLS\n    surface: CitiConnect (corporate Treasury and Trade Solutions)\n    note: >-\n      Client-certificate (mutual TLS) is required in addition to OAuth 2.0 for\n      CitiConnect enterprise connectivity, per Citi's published CitiConnect\n      documentation.\n    sources:\n      - apis.yml (citiconnect-api)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/citigroup/refs/heads/main/authentication/citigroup-authentication.yml
summary_line: oauth2/mutualTLS · 3 schemes
tags:
- Banking
- Financial-Services
- United States
- Money Center Bank
- Open Banking
- Open Finance
- Treasury and Trade Solutions
- CitiConnect
- Payments
- FX
- Corporate Banking
- Fortune 100
---
