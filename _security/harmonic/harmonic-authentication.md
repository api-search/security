---
api_key_in: []
auth_types:
- apiKey
description: The Aristotle API authenticates every request with a single API key. Keys are created in the Aristotle dashboard (sign in at https://aristotle.harmonic.fun, Dashboard -> API Keys). The official aristotlelib SDK/CLI reads the key from the ARISTOTLE_API_KEY environment variable or an explicit --api-key flag. There is no documented OAuth / OpenID Connect / scope surface — access is a single bearer secret per account. No OpenAPI is published, so this profile is captured from the provider's docs rather than derived from a spec.
kind: authentication
layout: security
method: searched
name: Harmonic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Harmonic secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Harmonic
provider_slug: harmonic
scheme_count: 1
schemes:
- description: Per-account API key created in the Aristotle dashboard and sent on every request over HTTPS. The exact HTTP header name is not publicly documented; the SDK supplies it from ARISTOTLE_API_KEY or --api-key.
  in: header
  name: aristotleApiKey
  sources:
  - https://aristotle.harmonic.fun/
  type: apiKey
slug: harmonic-authentication
source_filename: harmonic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://aristotle.harmonic.fun/ (Dashboard -> API Keys); https://pypi.org/project/aristotlelib/\ndescription: >-\n  The Aristotle API authenticates every request with a single API key. Keys are\n  created in the Aristotle dashboard (sign in at https://aristotle.harmonic.fun,\n  Dashboard -> API Keys). The official aristotlelib SDK/CLI reads the key from\n  the ARISTOTLE_API_KEY environment variable or an explicit --api-key flag. There\n  is no documented OAuth / OpenID Connect / scope surface — access is a single\n  bearer secret per account. No OpenAPI is published, so this profile is captured\n  from the provider's docs rather than derived from a spec.\nsummary:\n  types:\n  - apiKey\n  api_key_delivery:\n  - environment_variable: ARISTOTLE_API_KEY\n  - cli_flag: --api-key\n  oauth2_flows: []\nschemes:\n- name: aristotleApiKey\n  type: apiKey\n  description: >-\n    Per-account API key created in the Aristotle dashboard and\
  \ sent on every\n    request over HTTPS. The exact HTTP header name is not publicly documented;\n    the SDK supplies it from ARISTOTLE_API_KEY or --api-key.\n  in: header\n  sources:\n  - https://aristotle.harmonic.fun/\nkey_management:\n  create: https://aristotle.harmonic.fun (Dashboard -> API Keys)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/harmonic/refs/heads/main/authentication/harmonic-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
- Mathematics
- Formal Verification
- Theorem Proving
- Lean
- Machine Reasoning
- Developer Tools
---
