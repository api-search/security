---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kijito-ai-openapi-generated.yml
  format: yaml
  label: Kijito API
  slug: kijito-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kijito-ai/openapi/_ae-authored/kijito-ai-openapi-generated.yml
auth_types: []
description: 'Kijito supports two authentication methods: interactive sign‑in using OAuth and API‑key authentication via a Bearer token.'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Kijito Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kijito declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Kijito
provider_slug: kijito-ai
scheme_count: 1
schemes:
- evidence: Sign in with your account - for you, at the keyboard. The client opens a browser, you sign in to Kijito, and the client keeps the session.
  flows:
  - authorization_code
  how_to_obtain: Create an account, then run the client’s login command which opens a sign‑in link; after signing in the client stores the session.
  name: Sign in with your account
  scopes:
  - memory.read
  - memory.write
  - memory.curate
  - memory.dream
  type: oauth2
slug: kijito-ai-authentication
source_filename: kijito-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://kijito.ai/docs/quickstart
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://kijito.ai/docs/quickstart\nsources:\n- https://kijito.ai/docs/quickstart\ndescription: 'Kijito supports two authentication methods: interactive sign‑in using OAuth and API‑key authentication via a Bearer token.'\nschemes:\n- type: oauth2\n  name: Sign in with your account\n  evidence: Sign in with your account - for you, at the keyboard. The client opens a browser, you sign in to Kijito, and the client keeps the\n    session.\n  flows:\n  - authorization_code\n  scopes:\n  - memory.read\n  - memory.write\n  - memory.curate\n  - memory.dream\n  how_to_obtain: Create an account, then run the client’s login command which opens a sign‑in link; after signing in the client stores the session.\ndocs: https://kijito.ai/docs/quickstart\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/kijito-ai/authentication/kijito-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Memory
- Agents
- Productivity
- Platform
---
