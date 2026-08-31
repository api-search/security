---
api_key_in: []
api_specs:
- filename: browserstack-accesskey-api-openapi.yml
  format: yaml
  label: BrowserStack AccessKey API
  slug: browserstack-accesskey-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/openapi/browserstack-accesskey-api-openapi.yml
- filename: browserstack-browsers-api-openapi.yml
  format: yaml
  label: BrowserStack Browsers API
  slug: browserstack-browsers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/openapi/browserstack-browsers-api-openapi.yml
- filename: browserstack-builds-api-openapi.yml
  format: yaml
  label: BrowserStack Builds API
  slug: browserstack-builds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/openapi/browserstack-builds-api-openapi.yml
- filename: browserstack-plan-api-openapi.yml
  format: yaml
  label: BrowserStack Plan API
  slug: browserstack-plan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/openapi/browserstack-plan-api-openapi.yml
- filename: browserstack-projects-api-openapi.yml
  format: yaml
  label: BrowserStack Projects API
  slug: browserstack-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/openapi/browserstack-projects-api-openapi.yml
- filename: browserstack-sessions-api-openapi.yml
  format: yaml
  label: BrowserStack Sessions API
  slug: browserstack-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/openapi/browserstack-sessions-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Browserstack Authentication
name_suffix: Authentication
oauth_flows: []
overview: BrowserStack secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: BrowserStack
provider_slug: browserstack
scheme_count: 1
schemes:
- description: HTTP Basic auth using your BrowserStack username as username and your access key as password.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/browserstack-openapi.yml
  type: http
slug: browserstack-authentication
source_filename: browserstack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/browserstack-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using your BrowserStack username as username and your access\n    key as password.\n  sources:\n  - openapi/browserstack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/browserstack/refs/heads/main/authentication/browserstack-authentication.yml
summary_line: http · 1 scheme
tags:
- Accessibility
- Appium
- Application
- Automation
- CI/CD
- Cross-Browser Testing
- Enterprise
- JavaScript
- Low Code
- Mobile Testing
- QA
- Regression Testing
- Selenium
- Testing
- Unit Testing
- Visual Testing
---
