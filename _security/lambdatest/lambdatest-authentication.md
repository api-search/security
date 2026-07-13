---
api_key_in: []
api_specs:
- filename: index.html
  format: yaml
  label: LambdaTest Web Automation API
  slug: web-automation-api
  spec_type: OpenAPI
  url: https://swagger-api-support.lambdatest.com/index.html
- filename: index.html
  format: yaml
  label: LambdaTest SmartUI API
  slug: smartui-api
  spec_type: OpenAPI
  url: https://swagger-api-support.lambdatest.com/smartui/index.html
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Lambdatest Authentication
name_suffix: Authentication
oauth_flows: []
overview: LambdaTest secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: LambdaTest
provider_slug: lambdatest
scheme_count: 1
schemes:
- name: basicAuth
  scheme: basic
  sources:
  - openapi/lambdatest-smartui-api-openapi.yml
  - openapi/lambdatest-web-automation-api-openapi.yml
  type: http
slug: lambdatest-authentication
source_filename: lambdatest-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lambdatest-smartui-api-openapi.yml, openapi/lambdatest-web-automation-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/lambdatest-smartui-api-openapi.yml\n  - openapi/lambdatest-web-automation-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lambdatest/refs/heads/main/authentication/lambdatest-authentication.yml
summary_line: http · 1 scheme
tags:
- Testing
- Cross-Browser Testing
- Selenium
- Cypress
- Playwright
- Mobile Testing
- Automation
- QA
- Visual Regression
---
