---
api_key_in:
- environment
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Vals Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vals Ai secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vals Ai
provider_slug: vals-ai
scheme_count: 1
schemes:
- description: API keys are created on the Admin page of the platform.vals.ai console (account signup + email confirmation required). The SDK and CLI read the key from the VALS_API_KEY environment variable, or it can be set programmatically via vals.configure_credentials(api_key=...).
  in: environment
  name: VALS_API_KEY
  sources:
  - https://docs.vals.ai/sdk/setup
  - https://docs.vals.ai/get_started/quickstart
  type: apiKey
slug: vals-ai-authentication
source_filename: vals-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.vals.ai/sdk/setup\ndocs: https://docs.vals.ai/cli/cli#authentication\nsummary:\n  types: [apiKey]\n  api_key_in: [environment]\n  oauth2_flows: []\nschemes:\n  - name: VALS_API_KEY\n    type: apiKey\n    in: environment\n    description: >-\n      API keys are created on the Admin page of the platform.vals.ai console\n      (account signup + email confirmation required). The SDK and CLI read the\n      key from the VALS_API_KEY environment variable, or it can be set\n      programmatically via vals.configure_credentials(api_key=...).\n    sources:\n      - https://docs.vals.ai/sdk/setup\n      - https://docs.vals.ai/get_started/quickstart\nregions:\n  - name: US (default)\n    endpoint: https://platform.vals.ai\n  - name: EU\n    how: 'export VALS_REGION=\"europe\" or configure_credentials(api_key=..., in_eu=True)'\n  - name: Custom deployment\n    how: 'export VALS_ENDPOINT=\"https://your-org.platform.vals.ai\"\
  \ or configure_credentials(endpoint=...)'\nnotes: >-\n  No public OpenAPI is published, so no securitySchemes could be derived from\n  a spec; this profile is captured from the SDK/CLI authentication docs. No\n  OAuth2/OIDC surface is documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vals-ai/refs/heads/main/authentication/vals-ai-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai
- Artificial Intelligence
- LLM
- Evaluation
- Benchmarks
- Model Testing
- Legal
- Finance
---
