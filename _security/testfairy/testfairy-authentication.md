---
api_key_in:
- header
- formData
auth_types:
- http
- bearer
- apiKey
description: TestFairy authenticates REST API calls with HTTP Basic auth using your account email as the username and your API key as the password, or with an OIDC bearer token (Sauce Labs single sign-on). The API key is found on the TestFairy account settings page. The Upload API additionally accepts the API key as an `api_key` multipart form field. No OAuth 2.0 authorization-code / scope surface is documented, so there is no scopes/ artifact for this provider.
kind: authentication
layout: security
method: searched
name: Testfairy Authentication
name_suffix: Authentication
oauth_flows: []
overview: TestFairy secures its APIs with http, bearer, and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: TestFairy
provider_slug: testfairy
scheme_count: 3
schemes:
- description: 'HTTP Basic authentication. Username = account email, password = API key. Example: curl -u "email:api-key" https://mobile.saucelabs.com/api/1/projects/'
  location: Authorization header
  name: basicAuth
  scheme: basic
  sources:
  - docs
  type: http
- description: 'OIDC bearer token issued through Sauce Labs SSO. Sent as `Authorization: Bearer <token>` together with an `X-OIDC-Config-Key` header identifying the OIDC configuration.'
  location: Authorization header + X-OIDC-Config-Key header
  name: oidcBearer
  scheme: bearer
  sources:
  - docs
  type: http
- description: 'The Upload API (POST /api/upload) accepts the API key as an `api_key` multipart form field: curl https://app.testfairy.com/api/upload -F api_key=''your_api_key'' -F file=@app.apk'
  in: formData
  name: uploadApiKey
  parameter_name: api_key
  sources:
  - docs
  type: apiKey
slug: testfairy-authentication
source_filename: testfairy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.saucelabs.com/testfairy/api-reference/rest-api/, https://docs.saucelabs.com/testfairy/api-reference/upload-api/\ndocs: https://docs.saucelabs.com/testfairy/api-reference/rest-api/\ndescription: >-\n  TestFairy authenticates REST API calls with HTTP Basic auth using your account\n  email as the username and your API key as the password, or with an OIDC bearer\n  token (Sauce Labs single sign-on). The API key is found on the TestFairy\n  account settings page. The Upload API additionally accepts the API key as an\n  `api_key` multipart form field. No OAuth 2.0 authorization-code / scope surface\n  is documented, so there is no scopes/ artifact for this provider.\nsummary:\n  types: [http, bearer, apiKey]\n  api_key_in: [header, formData]\n  oauth2_flows: []\nschemes:\n  - name: basicAuth\n    type: http\n    scheme: basic\n    description: >-\n      HTTP Basic authentication. Username = account email, password =\
  \ API key.\n      Example: curl -u \"email:api-key\" https://mobile.saucelabs.com/api/1/projects/\n    location: Authorization header\n    sources: [docs]\n  - name: oidcBearer\n    type: http\n    scheme: bearer\n    description: >-\n      OIDC bearer token issued through Sauce Labs SSO. Sent as\n      `Authorization: Bearer <token>` together with an `X-OIDC-Config-Key` header\n      identifying the OIDC configuration.\n    location: Authorization header + X-OIDC-Config-Key header\n    sources: [docs]\n  - name: uploadApiKey\n    type: apiKey\n    in: formData\n    parameter_name: api_key\n    description: >-\n      The Upload API (POST /api/upload) accepts the API key as an `api_key`\n      multipart form field: curl https://app.testfairy.com/api/upload -F\n      api_key='your_api_key' -F file=@app.apk\n    sources: [docs]\nnotes: >-\n  API keys are long-lived and account-scoped; rotate them from the TestFairy\n  settings page. There is no per-scope permission model exposed via the API\
  \ —\n  admin/tester access levels are managed through the dashboard permissions\n  surface (GET /api/1/cpanel/permissions/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/testfairy/refs/heads/main/authentication/testfairy-authentication.yml
summary_line: http/bearer/apiKey · 3 schemes
tags:
- Company
- Mobile
- Testing
- App Distribution
- Beta Testing
- Quality Assurance
- Developer Tools
- Session Recording
- Crash Reporting
- DevOps
---
