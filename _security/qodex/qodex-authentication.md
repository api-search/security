---
anonymous_access: false
api_key_in: []
api_specs:
- filename: qodex-openapi-generated.yml
  format: yaml
  label: QodexAI API
  slug: qodex-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/qodex/openapi/_ae-authored/qodex-openapi-generated.yml
auth_types: []
description: Authentication methods described by QodexAI documentation.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Qodex Authentication
name_suffix: Authentication
oauth_flows: []
overview: QodexAI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: QodexAI
provider_slug: qodex
scheme_count: 2
schemes:
- evidence: OAuth 2.0 is an open standard for access delegation, commonly used as a way for Internet users to grant websites or applications access to their information on other websites without sharing their passwords.
  name: OAuth 2.0
  type: oauth2
- evidence: 'The Rugcheck API uses Bearer Token Authentication . This means: Every request must include your API key in the header.'
  header: Authorization
  how_to_obtain: Obtain a bearer token (API key) from the Rugcheck dashboard after generating an API key.
  location: header
  name: Bearer Token
  type: http-bearer
slug: qodex-authentication
source_filename: qodex-authentication.yml
source_heading: Authentication Profile
source_url: https://qodex.ai/blog/10-api-authentication-best-practices-for-securing-apis
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://qodex.ai/blog/10-api-authentication-best-practices-for-securing-apis\nsources:\n- https://qodex.ai/blog/10-api-authentication-best-practices-for-securing-apis\n- https://qodex.ai/blog/15-api-security-best-practices-to-secure-your-apis-in-2026\n- https://qodex.ai/blog/how-to-get-a-rugcheck-api-key-and-start-using-the-api\n- https://qodex.ai/blog/what-is-api-authentication\ndescription: Authentication methods described by QodexAI documentation.\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: OAuth 2.0 is an open standard for access delegation, commonly used as a way for Internet users to grant websites or applications access\n    to their information on other websites without sharing their passwords.\n- type: http-bearer\n  name: Bearer Token\n  evidence: 'The Rugcheck API uses Bearer Token Authentication . This means: Every request must include your API key in the\
  \ header.'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a bearer token (API key) from the Rugcheck dashboard after generating an API key.\ndocs: https://qodex.ai/blog/10-api-authentication-best-practices-for-securing-apis\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/qodex/authentication/qodex-authentication.yml
summary_line: 2 schemes
tags:
- Company
- AI
- Testing
- Continuous Integration
- DevOps
---
