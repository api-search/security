---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Pardot Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Salesforce Marketing Cloud Account Engagement (Pardot) secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Salesforce Marketing Cloud Account Engagement (Pardot)
provider_slug: pardot
scheme_count: 1
schemes:
- description: 'Authenticate via Salesforce OAuth2 and pass the resulting access

    token as `Authorization: Bearer {token}`. The `Pardot-Business-Unit-Id`

    header is also required on every request.'
  flows:
  - authorizationUrl: https://login.salesforce.com/services/oauth2/authorize
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://login.salesforce.com/services/oauth2/token
  name: BearerAuth
  sources:
  - openapi/pardot-openapi.yml
  type: oauth2
slug: pardot-authentication
source_filename: pardot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/pardot-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: BearerAuth\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://login.salesforce.com/services/oauth2/authorize\n    tokenUrl: https://login.salesforce.com/services/oauth2/token\n    scopes: 1\n  description: |-\n    Authenticate via Salesforce OAuth2 and pass the resulting access\n    token as `Authorization: Bearer {token}`. The `Pardot-Business-Unit-Id`\n    header is also required on every request.\n  sources:\n  - openapi/pardot-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pardot/refs/heads/main/authentication/pardot-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Marketing Automation
- B2B Marketing
- Lead Generation
- Email Marketing
- Salesforce
- Account Engagement
---
