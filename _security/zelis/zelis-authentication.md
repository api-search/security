---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Zelis Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Zelis secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Zelis
provider_slug: zelis
scheme_count: 2
schemes:
- credentials:
    client_id: unique identifier for the API client
    client_secret: client secret, valid for one year, authenticates the API client
    tenant_id: optional exclusive identifier for an organization within Zelis
  flow: clientCredentials
  name: oauth2ClientCredentials
  source: docs
  token_ttl_seconds: 3600
  token_url: https://api.zelis.com/auth/token
  type: oauth2
- description: Azure API Management subscription key that identifies the calling application; issued in the developer portal under Profile > My Account > Access Keys.
  in: header
  name: subscriptionKey
  parameter_name: Ocp-Apim-Subscription-Key
  source: docs
  type: apiKey
slug: zelis-authentication
source_filename: zelis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://developer.zelis.com/guides/getting-started-guests\ndocs: https://developer.zelis.com/guides/getting-started-guests\nsummary:\n  types:\n  - oauth2\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  notes: >-\n    Zelis API access requires TWO credentials on every call: an OAuth2 bearer\n    token obtained via the client-credentials grant, plus an Azure API\n    Management subscription key sent in the Ocp-Apim-Subscription-Key header.\n    All requests are HTTPS-only with JSON payloads.\nschemes:\n- name: oauth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: https://api.zelis.com/auth/token\n  token_ttl_seconds: 3600\n  credentials:\n    client_id: unique identifier for the API client\n    client_secret: client secret, valid for one year, authenticates the API client\n    tenant_id: optional exclusive identifier for an organization within Zelis\n  source: docs\n\
  - name: subscriptionKey\n  type: apiKey\n  in: header\n  parameter_name: Ocp-Apim-Subscription-Key\n  description: >-\n    Azure API Management subscription key that identifies the calling\n    application; issued in the developer portal under Profile > My Account >\n    Access Keys.\n  source: docs\nonboarding:\n  steps:\n  - Register via the developer-portal signup form (business email required)\n  - Confirm email address within 48 hours\n  - Zelis team reviews and approves the request\n  - Receive a temporary password (expires in 48 hours) and set a new password on first login\n  - Retrieve access keys under Profile > My Account > Access Keys\n  signup_url: https://devportalsignup.zelis.com/\nenvironments:\n- production\n- sandbox (where available per product)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zelis/refs/heads/main/authentication/zelis-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Company
- Healthcare
- Healthcare Payments
- Claims
- Payments
- Price Transparency
- Provider Directory
- Member Engagement
- Insurance
- FinTech
---
