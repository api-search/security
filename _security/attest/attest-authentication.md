---
anonymous_access: false
api_key_in: []
api_specs:
- filename: attest-openapi-generated.yml
  format: yaml
  label: Attest API
  slug: attest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/attest/refs/heads/main/openapi/_ae-authored/attest-openapi-generated.yml
auth_types: []
description: Attest uses a simple API key authentication scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Attest Authentication
name_suffix: Authentication
oauth_flows: []
overview: Attest declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Attest
provider_slug: attest
scheme_count: 1
schemes:
- evidence: 'Pass your API key in the `X-API-Key` header on every request:'
  header: X-API-Key
  how_to_obtain: Log in to your Attest account, navigate to **API & MCP** on the main nav, scroll to the **API key** section, click **Create API key**, then copy the generated key.
  location: header
  name: API Key
  type: apiKey
slug: attest-authentication
source_filename: attest-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.askattest.com/docs/authentication.md
source_yaml: "generated: '2026-09-26'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.askattest.com/docs/authentication.md\nsources:\n- https://developers.askattest.com/docs/authentication.md\n- https://developers.askattest.com/docs/authentication\n- https://help.askattest.com/en/articles/3494059-getting-started-with-your-first-survey\n- https://help.askattest.com/en/articles/5951282-getting-started-with-the-attest-platform\ndescription: Attest uses a simple API key authentication scheme.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Pass your API key in the `X-API-Key` header on every request:'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Log in to your Attest account, navigate to **API & MCP** on the main nav, scroll to the **API key** section, click **Create API\n    key**, then copy the generated key.\nnote: No OAuth2, HTTP Bearer, or other authentication methods are documented.\ndocs: https://developers.askattest.com/docs/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attest/refs/heads/main/authentication/attest-authentication.yml
summary_line: 1 scheme
tags:
- AI
- ConsumerInsights
- MarketResearch
- B2C
- Analytics
---
