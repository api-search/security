---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Chargeautomation Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChargeAutomation declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ChargeAutomation
provider_slug: chargeautomation
scheme_count: 1
schemes:
- description: Token based client credentials flow
  flows:
    clientCredentials:
      scopes: []
      tokenUrl: https://api.chargeautomation.com/api/v1/oauth/token
  type: oauth2
slug: chargeautomation-authentication
source_filename: chargeautomation-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://api.chargeautomation.com/docs/\nschemes:\n  - type: oauth2\n    description: Token based client credentials flow\n    flows:\n      clientCredentials:\n        tokenUrl: https://api.chargeautomation.com/api/v1/oauth/token\n        scopes: []\n"
source_yaml_url: https://artifacts.apis.io/chargeautomation/authentication/chargeautomation-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Hospitality
- Guest Experience
- Payments
- Property Management
---
