---
anonymous_access: false
api_key_in: []
api_specs:
- filename: glasswarp-com-agent-api-openapi.yml
  format: yaml
  label: glasswarp-com Agent API
  slug: glasswarp-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-agent-api-openapi.yml
- filename: glasswarp-com-api-keys-api-openapi.yml
  format: yaml
  label: glasswarp-com API Keys API
  slug: glasswarp-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-api-keys-api-openapi.yml
- filename: glasswarp-com-apps-api-openapi.yml
  format: yaml
  label: glasswarp-com Apps API
  slug: glasswarp-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-apps-api-openapi.yml
- filename: glasswarp-com-grounding-api-openapi.yml
  format: yaml
  label: glasswarp-com Grounding API
  slug: glasswarp-com-grounding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-grounding-api-openapi.yml
- filename: glasswarp-com-input-api-openapi.yml
  format: yaml
  label: glasswarp-com Input API
  slug: glasswarp-com-input-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-input-api-openapi.yml
- filename: glasswarp-com-rigs-api-openapi.yml
  format: yaml
  label: glasswarp-com Rigs API
  slug: glasswarp-com-rigs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-rigs-api-openapi.yml
- filename: glasswarp-com-screenshots-api-openapi.yml
  format: yaml
  label: glasswarp-com Screenshots API
  slug: glasswarp-com-screenshots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-screenshots-api-openapi.yml
- filename: glasswarp-com-sessions-api-openapi.yml
  format: yaml
  label: glasswarp-com Sessions API
  slug: glasswarp-com-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-sessions-api-openapi.yml
- filename: glasswarp-com-streaming-api-openapi.yml
  format: yaml
  label: glasswarp-com Streaming API
  slug: glasswarp-com-streaming-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-streaming-api-openapi.yml
- filename: glasswarp-com-webhooks-api-openapi.yml
  format: yaml
  label: glasswarp-com Webhooks API
  slug: glasswarp-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/glasswarp-com/openapi/glasswarp-com-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes for Glasswarp API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Glasswarp Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: glasswarp-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: glasswarp-com
provider_slug: glasswarp-com
scheme_count: 2
schemes:
- evidence: 'Most `/v1/*` endpoints require a bearer token:


    ```

    Authorization: Bearer gw_live_sk_...

    ```'
  header: Authorization
  how_to_obtain: API keys are created in the Console
  location: header
  name: apiKey
  type: http-bearer
- evidence: Supabase user JWT (for console/dashboard endpoints)
  header: Authorization
  how_to_obtain: Supabase user JWT (for console/dashboard endpoints)
  location: header
  name: userJwt
  type: http-bearer
slug: glasswarp-com-authentication
source_filename: glasswarp-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.glasswarp.com/api-reference/api-keys/list-api-keys.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.glasswarp.com/api-reference/api-keys/list-api-keys.md\nsources:\n- https://docs.glasswarp.com/api-reference/api-keys/list-api-keys.md\n- https://docs.glasswarp.com/api-reference/api-keys/create-an-api-key.md\n- https://docs.glasswarp.com/api-reference/api-keys/revoke-an-api-key.md\n- https://docs.glasswarp.com/quickstart.md\ndescription: Authentication schemes for Glasswarp API\nschemes:\n- type: http-bearer\n  name: apiKey\n  evidence: 'Most `/v1/*` endpoints require a bearer token:\n\n\n    ```\n\n    Authorization: Bearer gw_live_sk_...\n\n    ```'\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are created in the Console\n- type: http-bearer\n  name: userJwt\n  evidence: Supabase user JWT (for console/dashboard endpoints)\n  location: header\n  header: Authorization\n  how_to_obtain: Supabase user JWT (for console/dashboard endpoints)\ndocs:\
  \ https://docs.glasswarp.com/api-reference/api-keys/list-api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/glasswarp-com/authentication/glasswarp-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API
- Automation
- Windows
- RPA
---
