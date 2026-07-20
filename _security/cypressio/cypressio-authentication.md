---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Cypressio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cypress.io secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cypress.io
provider_slug: cypressio
scheme_count: 2
schemes:
- applies_to: Cypress Cloud Data Extract API (enterprise reporting)
  in: query
  name: OrganizationApiKey
  parameter: token
  provisioning: An organization API key is generated under Integrations -> Enterprise API in Cypress Cloud and passed on every request as the `token` query parameter.
  scope: Enterprise plan subscription required.
  sources:
  - https://docs.cypress.io/cloud/integrations/data-extract-api
  type: apiKey
- applies_to: Recording test runs to Cypress Cloud (cypress run --record --key)
  in: other
  name: RecordKey
  parameter: record key
  provisioning: A per-project record key issued in Cypress Cloud, supplied to the runner via --key or the CYPRESS_RECORD_KEY environment variable. Not part of the REST reporting API; documented here for completeness.
  sources:
  - https://docs.cypress.io/app/references/command-line
  type: apiKey
slug: cypressio-authentication
source_filename: cypressio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.cypress.io/cloud/integrations/data-extract-api\ndocs: https://docs.cypress.io/cloud/integrations/data-extract-api\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\nschemes:\n- name: OrganizationApiKey\n  type: apiKey\n  in: query\n  parameter: token\n  applies_to: Cypress Cloud Data Extract API (enterprise reporting)\n  provisioning: >-\n    An organization API key is generated under Integrations -> Enterprise API in\n    Cypress Cloud and passed on every request as the `token` query parameter.\n  scope: Enterprise plan subscription required.\n  sources: [https://docs.cypress.io/cloud/integrations/data-extract-api]\n- name: RecordKey\n  type: apiKey\n  in: other\n  parameter: record key\n  applies_to: Recording test runs to Cypress Cloud (cypress run --record --key)\n  provisioning: >-\n    A per-project record key issued in Cypress Cloud, supplied to the runner via\n    --key or the CYPRESS_RECORD_KEY\
  \ environment variable. Not part of the REST\n    reporting API; documented here for completeness.\n  sources: [https://docs.cypress.io/app/references/command-line]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cypressio/refs/heads/main/authentication/cypressio-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Testing
- End-to-End Testing
- Test Automation
- Quality Assurance
- Developer Tools
- CI/CD
- Accessibility
- JavaScript
---
