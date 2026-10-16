---
anonymous_access: false
api_key_in: []
api_specs:
- filename: entrypointai-openapi-generated.yml
  format: yaml
  label: Entry Point AI API
  slug: entrypointai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/entrypointai/refs/heads/main/openapi/_ae-authored/entrypointai-openapi-generated.yml
auth_types: []
description: Authentication schemes for Entry Point AI (as documented).
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Entrypointai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Entry Point AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Entry Point AI
provider_slug: entrypointai
scheme_count: 1
schemes:
- evidence: The Termly API uses API keys to authenticate requests.
  how_to_obtain: Keys are issued manually; contact https://termly.io/agencies/ to get access.
  name: API Key
  type: apiKey
slug: entrypointai-authentication
source_filename: entrypointai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.termly.io/introduction/authentication/
source_yaml: "generated: '2026-10-16'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.termly.io/introduction/authentication/\nsources:\n- https://docs.termly.io/introduction/authentication/\n- https://docs.entrypointai.com/getting-started/introduction.md\n- https://docs.entrypointai.com/getting-started/quickstart.md\n- https://docs.entrypointai.com/getting-started/quickstart\ndescription: Authentication schemes for Entry Point AI (as documented).\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: The Termly API uses API keys to authenticate requests.\n  how_to_obtain: Keys are issued manually; contact https://termly.io/agencies/ to get access.\ndocs: https://docs.termly.io/introduction/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entrypointai/refs/heads/main/authentication/entrypointai-authentication.yml
summary_line: 1 scheme
tags:
- AI
- Platform
- Machine Learning
- Data Engineering
- SaaS
---
