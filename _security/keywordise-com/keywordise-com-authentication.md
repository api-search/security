---
anonymous_access: false
api_key_in: []
auth_types: []
description: Keywordise supports OAuth and API key authentication for connecting AI assistants.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Keywordise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keywordise declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Keywordise
provider_slug: keywordise-com
scheme_count: 2
schemes:
- evidence: 'Assistants sign in with OAuth: you log in to Keywordise and approve.'
  how_to_obtain: Log in to Keywordise and approve the sign‑in request.
  name: OAuth
  type: oauth2
- evidence: If an assistant asks for a key instead, create one in your settings under API keys and give it only to the assistant's own credential prompt.
  how_to_obtain: Create an API key in the Keywordise settings under API keys.
  name: API key
  type: apiKey
slug: keywordise-com-authentication
source_filename: keywordise-com-authentication.yml
source_heading: Authentication Profile
source_url: https://keywordise.com/apply-with-ai
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://keywordise.com/apply-with-ai\nsources:\n- https://keywordise.com/apply-with-ai\ndescription: Keywordise supports OAuth and API key authentication for connecting AI assistants.\nschemes:\n- type: oauth2\n  name: OAuth\n  evidence: 'Assistants sign in with OAuth: you log in to Keywordise and approve.'\n  how_to_obtain: Log in to Keywordise and approve the sign‑in request.\n- type: apiKey\n  name: API key\n  evidence: If an assistant asks for a key instead, create one in your settings under API keys and give it only to the assistant's own credential\n    prompt.\n  how_to_obtain: Create an API key in the Keywordise settings under API keys.\ndocs: https://keywordise.com/apply-with-ai\n"
source_yaml_url: https://artifacts.apis.io/keywordise-com/authentication/keywordise-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Job Search
- Automation
- CVTailoring
- Software-as-a-Service
---
