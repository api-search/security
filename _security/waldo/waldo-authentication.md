---
api_key_in:
- header
- environment
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Waldo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Waldo secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Waldo
provider_slug: waldo
scheme_count: 1
schemes:
- description: 'Waldo authenticates API and CLI access with an API token. Two token scopes exist: a user-scoped token for development (found in the Profile tab of account settings) and an application-scoped CI token (found in the General tab of the app Configuration). For the WebdriverIO service the token is supplied via the WALDO_API_TOKEN environment variable or the `key` option in wdio.conf; the CLI supplies it via `waldo auth` or at install time.'
  env_var: WALDO_API_TOKEN
  name: WaldoApiToken
  sources:
  - docs.waldo.com/reference/authentication
  - github.com/waldoapp/wdio-service
  token_scopes:
  - location: Profile tab (account settings)
    name: user
    use: development / local runs
  - location: General tab (app Configuration)
    name: ci
    use: CI/CD pipelines
  type: apiKey
slug: waldo-authentication
source_filename: waldo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.waldo.com/reference/authentication\ndocs: https://docs.waldo.com/reference/authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [header, environment]\n  oauth2_flows: []\nschemes:\n  - name: WaldoApiToken\n    type: apiKey\n    description: >-\n      Waldo authenticates API and CLI access with an API token. Two token scopes exist: a\n      user-scoped token for development (found in the Profile tab of account settings) and an\n      application-scoped CI token (found in the General tab of the app Configuration). For the\n      WebdriverIO service the token is supplied via the WALDO_API_TOKEN environment variable or\n      the `key` option in wdio.conf; the CLI supplies it via `waldo auth` or at install time.\n    token_scopes:\n      - name: user\n        location: Profile tab (account settings)\n        use: development / local runs\n      - name: ci\n        location: General tab (app Configuration)\n \
  \       use: CI/CD pipelines\n    env_var: WALDO_API_TOKEN\n    sources: [docs.waldo.com/reference/authentication, github.com/waldoapp/wdio-service]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/waldo/refs/heads/main/authentication/waldo-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Devops
- Testing
- Mobile
- Test Automation
- Quality Engineering
- WebDriver
- Appium
- CI/CD
---
