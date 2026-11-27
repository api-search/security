---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes used by EvalEgress as described in its guides.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: EvalEgress (Ingenious AI) Authentication
name_suffix: Authentication
oauth_flows: []
overview: EvalEgress (Ingenious AI) declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: EvalEgress (Ingenious AI)
provider_slug: evalscope-getingeniousai-com
scheme_count: 3
schemes:
- evidence: A service API key is a bearer credential a platform issues so programs can call its API as your account — model-provider keys with the sk- prefix are the common case in eval work.
  header: Authorization
  how_to_obtain: Rotate the key at the provider and load it from a secrets manager or environment variable at runtime.
  location: header
  name: generic_api_key
  type: http-bearer
- evidence: The token authenticates as its owner with whatever scopes it was granted, and eval folders are copied, committed and shared more casually than the repos the token unlocks.
  header: Authorization
  how_to_obtain: Revoke the token in GitHub settings and replace it with a short‑lived credential or a secrets‑manager entry.
  location: header
  name: github_token
  type: http-bearer
- evidence: 'A JWT is a bearer credential: whoever presents it is believed, and its payload states its own permissions and expiry in readable form.'
  header: Authorization
  how_to_obtain: Revoke or rotate the token at the issuer, shorten its lifetime, and obtain a new token at runtime via a service account.
  location: header
  name: jwt_token
  type: http-bearer
slug: evalscope-getingeniousai-com-authentication
source_filename: evalscope-getingeniousai-com-authentication.yml
source_heading: Authentication Profile
source_url: https://evalscope.getingeniousai.com/guides/api-key-declared-in-eval-configuration
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://evalscope.getingeniousai.com/guides/api-key-declared-in-eval-configuration\nsources:\n- https://evalscope.getingeniousai.com/guides/api-key-declared-in-eval-configuration\n- https://evalscope.getingeniousai.com/guides/github-token-in-an-eval-repo\n- https://evalscope.getingeniousai.com/guides/jwt-token-declared-in-eval-environment\n- https://evalscope.getingeniousai.com/guides/secrets-manager-for-eval-credentials\ndescription: Authentication schemes used by EvalEgress as described in its guides.\nschemes:\n- type: http-bearer\n  name: generic_api_key\n  evidence: A service API key is a bearer credential a platform issues so programs can call its API as your account — model-provider keys with\n    the sk- prefix are the common case in eval work.\n  location: header\n  header: Authorization\n  how_to_obtain: Rotate the key at the provider and load it from a secrets manager\
  \ or environment variable at runtime.\n- type: http-bearer\n  name: github_token\n  evidence: The token authenticates as its owner with whatever scopes it was granted, and eval folders are copied, committed and shared more casually\n    than the repos the token unlocks.\n  location: header\n  header: Authorization\n  how_to_obtain: Revoke the token in GitHub settings and replace it with a short‑lived credential or a secrets‑manager entry.\n- type: http-bearer\n  name: jwt_token\n  evidence: 'A JWT is a bearer credential: whoever presents it is believed, and its payload states its own permissions and expiry in readable\n    form.'\n  location: header\n  header: Authorization\n  how_to_obtain: Revoke or rotate the token at the issuer, shorten its lifetime, and obtain a new token at runtime via a service account.\ndocs: https://evalscope.getingeniousai.com/guides/api-key-declared-in-eval-configuration\n"
source_yaml_url: https://artifacts.apis.io/evalscope-getingeniousai-com/authentication/evalscope-getingeniousai-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Artificial Intelligence
- Security
- Data Protection
- Monitoring
---
