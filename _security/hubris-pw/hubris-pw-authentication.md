---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hubris-pw-audio-api-openapi.yml
  format: yaml
  label: Hubris Audio API
  slug: hubris-pw-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-audio-api-openapi.yml
- filename: hubris-pw-decisions-api-openapi.yml
  format: yaml
  label: Hubris Decisions API
  slug: hubris-pw-decisions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-decisions-api-openapi.yml
- filename: hubris-pw-embeddings-api-openapi.yml
  format: yaml
  label: Hubris Embeddings API
  slug: hubris-pw-embeddings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-embeddings-api-openapi.yml
- filename: hubris-pw-images-api-openapi.yml
  format: yaml
  label: Hubris Images API
  slug: hubris-pw-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-images-api-openapi.yml
- filename: hubris-pw-integrations-api-openapi.yml
  format: yaml
  label: Hubris Integrations API
  slug: hubris-pw-integrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-integrations-api-openapi.yml
- filename: hubris-pw-management-api-openapi.yml
  format: yaml
  label: Hubris Management API
  slug: hubris-pw-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-management-api-openapi.yml
- filename: hubris-pw-messages-api-openapi.yml
  format: yaml
  label: Hubris Messages API
  slug: hubris-pw-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-messages-api-openapi.yml
- filename: hubris-pw-metrics-api-openapi.yml
  format: yaml
  label: Hubris Metrics API
  slug: hubris-pw-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-metrics-api-openapi.yml
- filename: hubris-pw-models-api-openapi.yml
  format: yaml
  label: Hubris Models API
  slug: hubris-pw-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-models-api-openapi.yml
- filename: hubris-pw-rerank-api-openapi.yml
  format: yaml
  label: Hubris Rerank API
  slug: hubris-pw-rerank-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-rerank-api-openapi.yml
- filename: hubris-pw-responses-api-openapi.yml
  format: yaml
  label: Hubris Responses API
  slug: hubris-pw-responses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-responses-api-openapi.yml
- filename: hubris-pw-usage-api-openapi.yml
  format: yaml
  label: Hubris Usage API
  slug: hubris-pw-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-usage-api-openapi.yml
- filename: hubris-pw-videos-api-openapi.yml
  format: yaml
  label: Hubris Videos API
  slug: hubris-pw-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-videos-api-openapi.yml
- filename: hubris-pw-chat-completions-api-openapi.yml
  format: yaml
  label: Hubris Chat Completions API
  slug: hubris-pw-chat-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hubris-pw/openapi/hubris-pw-chat-completions-api-openapi.yml
auth_types: []
description: 'Hubris supports two authentication methods: API‑key (Bearer token) and OAuth 2.0 Authorization Code with PKCE.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hubris Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hubris declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hubris
provider_slug: hubris-pw
scheme_count: 2
schemes:
- evidence: 'Все запросы к Hubris авторизуются API-ключом в заголовке Authorization: Bearer sk-gw-<32-hex> .'
  header: Authorization
  how_to_obtain: Создайте ключ в UI по адресу /keys; ключ имеет префикс sk-gw- и 32 шестнадцатеричных символа.
  location: header
  name: API‑key
  type: http-bearer
- authorize_url: https://api.hubris.pw/oauth/authorize
  evidence: Hubris реализует OAuth 2.0 Authorization Code + PKCE (RFC 6749 + 7636, рекомендации RFC 9700) для авторизации сторонних приложений.
  header: Authorization
  how_to_obtain: Регистрация клиента происходит через endpoint https://api.hubris.pw/oauth/clients; клиент получает client_id (без client_secret) и использует PKCE для получения кода и обмена его на токен.
  location: header
  name: OAuth 2.0 Authorization Code + PKCE
  scopes:
  - chat:write
  - models:read
  - balance:read
  - videos:write
  - videos:read
  - offline_access
  token_url: https://api.hubris.pw/oauth/token
  type: oauth2
slug: hubris-pw-authentication
source_filename: hubris-pw-authentication.yml
source_heading: Authentication Profile
source_url: https://api.hubris.pw/.well-known/oauth-protected-resource
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.hubris.pw/.well-known/oauth-protected-resource\nsources:\n- https://api.hubris.pw/.well-known/oauth-protected-resource\n- https://hubris.pw/docs/integrations/oauth\n- https://hubris.pw/docs/authentication\n- https://hubris.pw/docs/quickstart.mdx\ndescription: 'Hubris supports two authentication methods: API‑key (Bearer token) and OAuth 2.0 Authorization Code with PKCE.'\nschemes:\n- type: http-bearer\n  name: API‑key\n  evidence: 'Все запросы к Hubris авторизуются API-ключом в заголовке Authorization: Bearer sk-gw-<32-hex> .'\n  location: header\n  header: Authorization\n  how_to_obtain: Создайте ключ в UI по адресу /keys; ключ имеет префикс sk-gw- и 32 шестнадцатеричных символа.\n- type: oauth2\n  name: OAuth 2.0 Authorization Code + PKCE\n  evidence: Hubris реализует OAuth 2.0 Authorization Code + PKCE (RFC 6749 + 7636, рекомендации RFC 9700) для авторизации сторонних\
  \ приложений.\n  location: header\n  header: Authorization\n  token_url: https://api.hubris.pw/oauth/token\n  authorize_url: https://api.hubris.pw/oauth/authorize\n  scopes:\n  - chat:write\n  - models:read\n  - balance:read\n  - videos:write\n  - videos:read\n  - offline_access\n  how_to_obtain: Регистрация клиента происходит через endpoint https://api.hubris.pw/oauth/clients; клиент получает client_id (без client_secret)\n    и использует PKCE для получения кода и обмена его на токен.\ndocs: https://api.hubris.pw/.well-known/oauth-protected-resource\n"
source_yaml_url: https://artifacts.apis.io/hubris-pw/authentication/hubris-pw-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Gateways
- Models
- OpenAI-Compatible
- Russian
---
