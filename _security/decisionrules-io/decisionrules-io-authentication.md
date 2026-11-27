---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication using API keys passed as Bearer tokens in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: DecisionRules Authentication
name_suffix: Authentication
oauth_flows: []
overview: DecisionRules declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: DecisionRules
provider_slug: decisionrules-io
scheme_count: 1
schemes:
- evidence: 'Authentication: When making a call to the Rule Solver API, the Solver API Key is typically included in the authorization header (e.g., `Authorization: Bearer <Solver API Key>`).'
  header: Authorization
  how_to_obtain: Create or retrieve the Solver API key from the API Keys page (Space → API Keys → Add API Key).
  location: header
  name: Solver API Key
  type: http-bearer
slug: decisionrules-io-authentication
source_filename: decisionrules-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.decisionrules.io/doc/api/api-keys.md
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.decisionrules.io/doc/api/api-keys.md\nsources:\n- https://docs.decisionrules.io/doc/api/api-keys.md\n- https://docs.decisionrules.io/doc/api/api-keys/solver-api-keys.md\n- https://docs.decisionrules.io/doc/api/api-keys/management-api-keys.md\n- https://docs.decisionrules.io/doc/api/api-keys/management-api-keys-1.md\ndescription: Authentication using API keys passed as Bearer tokens in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Solver API Key\n  evidence: 'Authentication: When making a call to the Rule Solver API, the Solver API Key is typically included in the authorization header (e.g.,\n    `Authorization: Bearer <Solver API Key>`).'\n  location: header\n  header: Authorization\n  how_to_obtain: Create or retrieve the Solver API key from the API Keys page (Space → API Keys → Add API Key).\nnote: Enterprise OAuth is mentioned but no concrete\
  \ OAuth flow details (token/authorize URLs, scopes) are provided on these pages.\ndocs: https://docs.decisionrules.io/doc/api/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/decisionrules-io/authentication/decisionrules-io-authentication.yml
summary_line: 1 scheme
tags:
- Business Rules
- Artificial Intelligence
- Enterprise
- Integration
- Low-Code
---
