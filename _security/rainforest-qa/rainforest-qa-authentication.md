---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: rainforest-qa-callback-api-openapi.yml
  format: yaml
  label: Rainforest QA Callback API
  slug: rainforest-qa-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-callback-api-openapi.yml
- filename: rainforest-qa-clients-api-openapi.yml
  format: yaml
  label: Rainforest QA Clients API
  slug: rainforest-qa-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-clients-api-openapi.yml
- filename: rainforest-qa-connections-api-openapi.yml
  format: yaml
  label: Rainforest QA Connections API
  slug: rainforest-qa-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-connections-api-openapi.yml
- filename: rainforest-qa-credit-cards-api-openapi.yml
  format: yaml
  label: Rainforest QA Credit Cards API
  slug: rainforest-qa-credit-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-credit-cards-api-openapi.yml
- filename: rainforest-qa-environments-api-openapi.yml
  format: yaml
  label: Rainforest QA Environments API
  slug: rainforest-qa-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-environments-api-openapi.yml
- filename: rainforest-qa-features-api-openapi.yml
  format: yaml
  label: Rainforest QA Features API
  slug: rainforest-qa-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-features-api-openapi.yml
- filename: rainforest-qa-folders-api-openapi.yml
  format: yaml
  label: Rainforest QA Folders API
  slug: rainforest-qa-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-folders-api-openapi.yml
- filename: rainforest-qa-generators-api-openapi.yml
  format: yaml
  label: Rainforest QA Generators API
  slug: rainforest-qa-generators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-generators-api-openapi.yml
- filename: rainforest-qa-on-premise-crowd-api-openapi.yml
  format: yaml
  label: Rainforest QA On Premise Crowd API
  slug: rainforest-qa-on-premise-crowd-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-on-premise-crowd-api-openapi.yml
- filename: rainforest-qa-run-groups-api-openapi.yml
  format: yaml
  label: Rainforest QA Run Groups API
  slug: rainforest-qa-run-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-run-groups-api-openapi.yml
- filename: rainforest-qa-runs-api-openapi.yml
  format: yaml
  label: Rainforest QA Runs API
  slug: rainforest-qa-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-runs-api-openapi.yml
- filename: rainforest-qa-site-environments-api-openapi.yml
  format: yaml
  label: Rainforest QA Site Environments API
  slug: rainforest-qa-site-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-site-environments-api-openapi.yml
- filename: rainforest-qa-sites-api-openapi.yml
  format: yaml
  label: Rainforest QA Sites API
  slug: rainforest-qa-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-sites-api-openapi.yml
- filename: rainforest-qa-tags-api-openapi.yml
  format: yaml
  label: Rainforest QA Tags API
  slug: rainforest-qa-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-tags-api-openapi.yml
- filename: rainforest-qa-test-results-api-openapi.yml
  format: yaml
  label: Rainforest QA Test Results API
  slug: rainforest-qa-test-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-test-results-api-openapi.yml
- filename: rainforest-qa-tests-api-openapi.yml
  format: yaml
  label: Rainforest QA Tests API
  slug: rainforest-qa-tests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-tests-api-openapi.yml
- filename: rainforest-qa-users-api-openapi.yml
  format: yaml
  label: Rainforest QA Users API
  slug: rainforest-qa-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-users-api-openapi.yml
- filename: rainforest-qa-vm-stack-api-openapi.yml
  format: yaml
  label: Rainforest QA Vm Stack API
  slug: rainforest-qa-vm-stack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/openapi/rainforest-qa-vm-stack-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Rainforest Qa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rainforest QA secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rainforest QA
provider_slug: rainforest-qa
scheme_count: 1
schemes:
- in: header
  name: api_key
  parameter: CLIENT_TOKEN
  sources:
  - openapi/rainforest-qa-openapi-original.yml
  type: apiKey
slug: rainforest-qa-authentication
source_filename: rainforest-qa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/rainforest-qa-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: CLIENT_TOKEN\n  sources:\n  - openapi/rainforest-qa-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rainforest-qa/refs/heads/main/authentication/rainforest-qa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Testing
- QA
- Test Automation
- Software Testing
- CI/CD
- Quality Assurance
- Crowdsourced Testing
- No-Code
- Developer Tools
---
