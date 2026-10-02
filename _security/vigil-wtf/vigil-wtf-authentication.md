---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes used by Vigil for Bedrock API access
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Vigil Wtf Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vigil declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Vigil
provider_slug: vigil-wtf
scheme_count: 2
schemes:
- evidence: 'Bedrock API keys have no body binding # Then AWS shipped Bedrock API keys — long-lived credentials sent as a plain header: Authorization: Bearer bedrock-api-key-...'
  header: Authorization
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'The signature lands in the Authorization header: Authorization: AWS4-HMAC-SHA256 Credential=.../bedrock/aws4_request, SignedHeaders=..., Signature=8f3a...'
  header: Authorization
  location: header
  name: SigV4
  type: other
slug: vigil-wtf-authentication
source_filename: vigil-wtf-authentication.yml
source_heading: Authentication Profile
source_url: https://www.vigil.wtf/blog/bedrock-api-keys-are-bearer-tokens
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.vigil.wtf/blog/bedrock-api-keys-are-bearer-tokens\nsources:\n- https://www.vigil.wtf/blog/bedrock-api-keys-are-bearer-tokens\n- https://www.vigil.wtf/tools/token-cost\n- https://www.vigil.wtf/blog/cache-minimums-why-nothing-below-1024-tokens-ever-caches\n- https://www.vigil.wtf/blog/fail-open-auth-when-a-missing-env-var-disables-your-security\ndescription: Authentication schemes used by Vigil for Bedrock API access\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Bedrock API keys have no body binding # Then AWS shipped Bedrock API keys — long-lived credentials sent as a plain header: Authorization:\n    Bearer bedrock-api-key-...'\n  location: header\n  header: Authorization\n- type: other\n  name: SigV4\n  evidence: 'The signature lands in the Authorization header: Authorization: AWS4-HMAC-SHA256 Credential=.../bedrock/aws4_request, SignedHeaders=...,\n\
  \    Signature=8f3a...'\n  location: header\n  header: Authorization\ndocs: https://www.vigil.wtf/blog/bedrock-api-keys-are-bearer-tokens\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vigil-wtf/refs/heads/main/authentication/vigil-wtf-authentication.yml
summary_line: 2 schemes
tags:
- Monitoring
- AI Middleware
- Security
- Analytics
---
