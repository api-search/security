---
anonymous_access: false
api_key_in: []
api_specs:
- filename: askmiles-ai-openapi-generated.yml
  format: yaml
  label: AskMiles AI API
  slug: askmiles-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/askmiles-ai/openapi/_ae-authored/askmiles-ai-openapi-generated.yml
auth_types: []
description: Authentication methods for AskMiles AI
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: AskMiles AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: AskMiles AI declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: AskMiles AI
provider_slug: askmiles-ai
scheme_count: 2
schemes:
- evidence: 'Send one request. curl https://askmiles.ai/v1/chat/completions \ -H "Authorization: Bearer $MILES_API_KEY" \ -H "Content-Type: application/json" \ -d ''{"model": "miles", "messages": [{"role": "user", "content": "Which card should I use at Costco?"}]}'''
  header: Authorization
  how_to_obtain: Mint a key in Settings → API keys; the key starts with miles_sk_ and is shown once.
  location: header
  name: Personal API key
  type: http-bearer
- authorize_url: https://mcp.askmiles.ai/authorize
  evidence: 'Register a client, send a user through consent, and call Miles on their behalf: the full OAuth 2.1 sequence, with every request and response.'
  header: Authorization
  how_to_obtain: Dynamic Client Registration via POST to https://mcp.askmiles.ai/register; the response returns a client_id which is the only credential the app holds.
  location: header
  name: OAuth app
  scopes:
  - miles:read
  - miles:chat
  - miles:write
  - miles:write:reconcile
  token_url: https://mcp.askmiles.ai/token
  type: oauth2
slug: askmiles-ai-authentication
source_filename: askmiles-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://askmiles.ai/docs/getting-started/personal-key?utm_source=llms&utm_medium=assistant
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://askmiles.ai/docs/getting-started/personal-key?utm_source=llms&utm_medium=assistant\nsources:\n- https://askmiles.ai/docs/getting-started/personal-key?utm_source=llms&utm_medium=assistant\n- https://askmiles.ai/docs/getting-started/oauth-app?utm_source=llms&utm_medium=assistant\n- https://askmiles.ai/docs/getting-started/personal-key\n- https://askmiles.ai/docs/getting-started/oauth-app\ndescription: Authentication methods for AskMiles AI\nschemes:\n- type: http-bearer\n  name: Personal API key\n  evidence: 'Send one request. curl https://askmiles.ai/v1/chat/completions \\ -H \"Authorization: Bearer $MILES_API_KEY\" \\ -H \"Content-Type: application/json\"\n    \\ -d ''{\"model\": \"miles\", \"messages\": [{\"role\": \"user\", \"content\": \"Which card should I use at Costco?\"}]}'''\n  location: header\n  header: Authorization\n  how_to_obtain: Mint a key in Settings → API\
  \ keys; the key starts with miles_sk_ and is shown once.\n- type: oauth2\n  name: OAuth app\n  evidence: 'Register a client, send a user through consent, and call Miles on their behalf: the full OAuth 2.1 sequence, with every request and\n    response.'\n  location: header\n  header: Authorization\n  token_url: https://mcp.askmiles.ai/token\n  authorize_url: https://mcp.askmiles.ai/authorize\n  scopes:\n  - miles:read\n  - miles:chat\n  - miles:write\n  - miles:write:reconcile\n  how_to_obtain: Dynamic Client Registration via POST to https://mcp.askmiles.ai/register; the response returns a client_id which is the only\n    credential the app holds.\ndocs: https://askmiles.ai/docs/getting-started/personal-key?utm_source=llms&utm_medium=assistant\n"
source_yaml_url: https://artifacts.apis.io/askmiles-ai/authentication/askmiles-ai-authentication.yml
summary_line: 2 schemes
tags:
- Fintech
- Credit Cards
- Rewards
- Personal Finance
- Artificial Intelligence
---
