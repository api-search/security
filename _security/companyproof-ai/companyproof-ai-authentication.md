---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Companyproof Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: companyproof-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: companyproof-ai
provider_slug: companyproof-ai
scheme_count: 1
schemes:
- description: API keys used as Bearer tokens. Keys begin with cp_test_ or cp_live_.
  header: 'Authorization: Bearer <API_KEY>'
  token_prefix: cp_test_ | cp_live_
  type: bearer
slug: companyproof-ai-authentication
source_filename: companyproof-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: searched\nsource: https://companyproof.ai/docs/authentication\nschemes:\n  - type: bearer\n    description: \"API keys used as Bearer tokens. Keys begin with cp_test_ or cp_live_.\"\n    token_prefix: \"cp_test_ | cp_live_\"\n    header: \"Authorization: Bearer <API_KEY>\"\n"
source_yaml_url: https://artifacts.apis.io/companyproof-ai/authentication/companyproof-ai-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Verification
- Compliance
- Data
- CompanyProof
---
