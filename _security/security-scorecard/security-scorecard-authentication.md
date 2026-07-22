---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Security Scorecard Authentication
name_suffix: Authentication
oauth_flows: []
overview: SecurityScorecard secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SecurityScorecard
provider_slug: security-scorecard
scheme_count: 1
schemes:
- example: 'Authorization: Token 1a1a1a1a1a1a1a1a'
  expires: false
  format: Token <api_key>
  in: header
  name: ApiTokenAuth
  parameter_name: Authorization
  sources:
  - docs
  token_generation: https://platform.securityscorecard.io/#/my-settings/api
  type: apiKey
slug: security-scorecard-authentication
source_filename: security-scorecard-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://securityscorecard.readme.io/docs/getting-started\ndocs: https://securityscorecard.readme.io/docs/getting-started\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    SecurityScorecard uses a static API-token scheme. Requests carry an\n    Authorization header whose value is the literal prefix \"Token\" followed by a\n    space and the API key. API keys do not expire and are as powerful as a\n    password, so they must be stored only in application secrets. Keys are\n    generated in the platform under My Settings > API; administrators can also\n    create bot (service-account) users that own keys scoped to an application.\nschemes:\n  - name: ApiTokenAuth\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    format: 'Token <api_key>'\n    example: 'Authorization: Token 1a1a1a1a1a1a1a1a'\n    token_generation: https://platform.securityscorecard.io/#/my-settings/api\n\
  \    expires: false\n    sources: [docs]\nservice_accounts:\n  supported: true\n  name: Bot user\n  docs: https://securityscorecard.readme.io/docs/create-bot-servicew-account-with-api-token\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/security-scorecard/refs/heads/main/authentication/security-scorecard-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise
- Cybersecurity
- Security Ratings
- Third-Party Risk
- Risk Management
- Attack Surface
- Compliance
---
