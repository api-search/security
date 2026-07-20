---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Convercent Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convercent secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Convercent
provider_slug: convercent
scheme_count: 1
schemes:
- applies_to:
  - https://api.convercent.com/OData/case/v5/CaseManagement.svc/
  - https://api.convercent.com/OData/v4/CampaignService.svc/
  description: HTTP Basic authentication using Convercent credentials (user name + password). Configured in OData/BI clients by selecting "Basic" and entering the Convercent user name and password.
  name: basicAuth
  scheme: basic
  sources:
  - docs
  type: http
slug: convercent-authentication
source_filename: convercent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://support.convercent.com/hc/en-us/articles/205259429-Convercent-OData-\ndocs: https://support.convercent.com/hc/en-us/articles/205259429-Convercent-OData-\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  notes: >-\n    The Convercent OData data-services API authenticates with HTTP Basic using a\n    Convercent user name and password. Access is licensed and restricted to\n    Administrators and Moderators of the respective domain; only those accounts\n    can consume the OData endpoints. There is no public OAuth or API-key surface\n    documented for the data API. (Application sign-in supports SAML SSO via\n    identity providers such as Okta, but that governs the web app, not the API.)\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication using Convercent credentials (user name +\n      password). Configured in OData/BI clients by selecting \"Basic\"\
  \ and\n      entering the Convercent user name and password.\n    applies_to:\n      - https://api.convercent.com/OData/case/v5/CaseManagement.svc/\n      - https://api.convercent.com/OData/v4/CampaignService.svc/\n    sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/convercent/refs/heads/main/authentication/convercent-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Saas
- Compliance
- Governance Risk And Compliance
- Ethics
- Case Management
- OData
- Reporting
---
