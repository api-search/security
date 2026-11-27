---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cybret-ai-openapi-generated.yml
  format: yaml
  label: CYBRET API
  slug: cybret-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cybret-ai/openapi/_ae-authored/cybret-ai-openapi-generated.yml
auth_types: []
description: Authentication schemes described in CYBRET research pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CYBRET Authentication
name_suffix: Authentication
oauth_flows: []
overview: CYBRET declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: CYBRET
provider_slug: cybret-ai
scheme_count: 2
schemes:
- evidence: Possession was treated as authorization, which is the default behavior of every bearer credential ever issued.
  header: Authorization
  how_to_obtain: Leaked API key found in a public GitHub repository; anonymous JWT obtained via POST /access/api/v1/aws/token/.
  location: header
  name: API Key / Bearer Token
  type: http-bearer
- evidence: Artifactory validates the token signature and issuer but does not properly enforce its intended scope.
  header: Authorization
  how_to_obtain: Send an unauthenticated POST to the token endpoint to receive an anonymous JWT.
  location: header
  name: Artifactory JWT
  token_url: /access/api/v1/aws/token/
  type: http-bearer
slug: cybret-ai-authentication
source_filename: cybret-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.cybret.ai/research/the-agent-found-the-api-key
source_yaml: "generated: '2026-11-04'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.cybret.ai/research/the-agent-found-the-api-key\nsources:\n- https://www.cybret.ai/research/the-agent-found-the-api-key\n- https://www.cybret.ai/research/they-checked-the-signature\ndescription: Authentication schemes described in CYBRET research pages.\nschemes:\n- type: http-bearer\n  name: API Key / Bearer Token\n  evidence: Possession was treated as authorization, which is the default behavior of every bearer credential ever issued.\n  location: header\n  header: Authorization\n  how_to_obtain: Leaked API key found in a public GitHub repository; anonymous JWT obtained via POST /access/api/v1/aws/token/.\n- type: http-bearer\n  name: Artifactory JWT\n  evidence: Artifactory validates the token signature and issuer but does not properly enforce its intended scope.\n  location: header\n  header: Authorization\n  token_url: /access/api/v1/aws/token/\n  how_to_obtain:\
  \ Send an unauthenticated POST to the token endpoint to receive an anonymous JWT.\nnote: No OAuth2 flows, apiKey, http-basic, or other authentication types were explicitly documented on the provided pages.\ndocs: https://www.cybret.ai/research/the-agent-found-the-api-key\n"
source_yaml_url: https://artifacts.apis.io/cybret-ai/authentication/cybret-ai-authentication.yml
summary_line: 2 schemes
tags:
- Security
- Penetration Testing
- API Security
- Software-as-a-Service
- Compliance
---
