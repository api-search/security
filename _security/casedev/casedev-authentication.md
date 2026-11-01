---
anonymous_access: false
api_key_in: []
api_specs:
- filename: casedev-api-openapi.json
  format: json
  label: Case.dev API API
  slug: case-dev-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/casedev/openapi/_original/casedev-api-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Casedev Authentication
name_suffix: Authentication
oauth_flows: []
overview: Case.dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Case.dev
provider_slug: casedev
scheme_count: 1
schemes:
- evidence: 'All requests require your API key in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Get your API key from the Console
  location: header
  name: API Key
  type: http-bearer
slug: casedev-authentication
source_filename: casedev-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.case.dev/connectors/oauth.md
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.case.dev/connectors/oauth.md\nsources:\n- https://docs.case.dev/connectors/oauth.md\n- https://docs.case.dev/api-reference/webhooks/rotate-webhook-signing-secret.md\n- https://docs.case.dev/getting-started/index.md\n- https://docs.case.dev/getting-started/discovery-search.md\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'All requests require your API key in the `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Get your API key from the Console\ndocs: https://docs.case.dev/connectors/oauth.md\n"
source_yaml_url: https://artifacts.apis.io/casedev/authentication/casedev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- LegalTech
- AI
- Platform
- Automation
---
