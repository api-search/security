---
anonymous_access: false
api_key_in: []
auth_types: []
description: Leen.dev's Authentication Method
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Leen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Leen declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Leen
provider_slug: leen
scheme_count: 2
schemes:
- evidence: Authentication is handled by two different headers, both are **required**.
  header: X-API-KEY
  location: header
  name: X-API-KEY
  type: apiKey
- evidence: Authentication is handled by two different headers, both are **required**.
  header: X-CONNECTION-ID
  location: header
  name: X-CONNECTION-ID
  type: apiKey
slug: leen-authentication
source_filename: leen-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.leen.dev/api-reference/authentication.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.leen.dev/api-reference/authentication.md\nsources:\n- https://docs.leen.dev/api-reference/authentication.md\n- https://docs.leen.dev/integrations/aws-access-analyzer-credentials.md\n- https://docs.leen.dev/api-reference/provisioning/test-connection.md\n- https://docs.leen.dev/api-reference/onramp/create-connection-invite-token.md\ndescription: Leen.dev's Authentication Method\nschemes:\n- type: apiKey\n  name: X-API-KEY\n  evidence: Authentication is handled by two different headers, both are **required**.\n  location: header\n  header: X-API-KEY\n- type: apiKey\n  name: X-CONNECTION-ID\n  evidence: Authentication is handled by two different headers, both are **required**.\n  location: header\n  header: X-CONNECTION-ID\nnote: Both headers are required for every request.\ndocs: https://docs.leen.dev/api-reference/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/leen/authentication/leen-authentication.yml
summary_line: 2 schemes
tags:
- Security
- API
- DataFabric
- Integration
- Automation
---
