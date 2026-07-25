---
api_key_in:
- header
api_specs:
- filename: amika-api-keys-api-openapi.yml
  format: yaml
  label: Amika API keys API
  slug: amika-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-api-keys-api-openapi.yml
- filename: amika-docker-registries-api-openapi.yml
  format: yaml
  label: Amika Docker registries API
  slug: amika-docker-registries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-docker-registries-api-openapi.yml
- filename: amika-downloads-api-openapi.yml
  format: yaml
  label: Amika Downloads API
  slug: amika-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-downloads-api-openapi.yml
- filename: amika-git-user-settings-api-openapi.yml
  format: yaml
  label: Amika Git user settings API
  slug: amika-git-user-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-git-user-settings-api-openapi.yml
- filename: amika-integrations-api-openapi.yml
  format: yaml
  label: Amika Integrations API
  slug: amika-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-integrations-api-openapi.yml
- filename: amika-repositories-api-openapi.yml
  format: yaml
  label: Amika Repositories API
  slug: amika-repositories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-repositories-api-openapi.yml
- filename: amika-sandboxes-api-openapi.yml
  format: yaml
  label: Amika Sandboxes API
  slug: amika-sandboxes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-sandboxes-api-openapi.yml
- filename: amika-sandboxsnapshots-api-openapi.yml
  format: yaml
  label: Amika SandboxSnapshots API
  slug: amika-sandboxsnapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-sandboxsnapshots-api-openapi.yml
- filename: amika-secrets-api-openapi.yml
  format: yaml
  label: Amika Secrets API
  slug: amika-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-secrets-api-openapi.yml
- filename: amika-services-api-openapi.yml
  format: yaml
  label: Amika Services API
  slug: amika-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-services-api-openapi.yml
- filename: amika-slack-api-openapi.yml
  format: yaml
  label: Amika Slack API
  slug: amika-slack-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-slack-api-openapi.yml
- filename: amika-uploads-api-openapi.yml
  format: yaml
  label: Amika Uploads API
  slug: amika-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/openapi/amika-uploads-api-openapi.yml
auth_types:
- http
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Amika Authentication
name_suffix: Authentication
oauth_flows:
- deviceAuthorization
overview: Amika secures its APIs with http, apiKey, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceAuthorization flow(s).
provider_name: Amika
provider_slug: amika
scheme_count: 4
schemes:
- description: 'Bearer token in the Authorization header. The token is either a long-lived API key created in the web UI (app.amika.dev/settings) or a short-lived access token minted by the OAuth device-authorization login flow. The CLI resolves credentials in precedence order: AMIKA_API_KEY env var, stored API key file (${XDG_STATE_HOME}/amika/api-key.json), then browser login session.'
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.amika.dev/reference/auth
  type: http
- description: API keys generated in the web UI for non-interactive/CI use. Provided via the AMIKA_API_KEY environment variable or on-disk key file, presented as a bearer token to the API. Managed through the /api-keys operations.
  in: header
  name: apiKey
  sources:
  - https://docs.amika.dev/reference/auth
  type: apiKey
- description: Interactive browser login for local development. The CLI requests a device code, the user authorizes in the browser, the CLI polls until complete, and a session is stored with access token, refresh token, email, and org. Tokens auto-refresh within 60 seconds of expiry. Identity is brokered by WorkOS.
  flow: deviceAuthorization
  name: deviceAuthorization
  sources:
  - https://docs.amika.dev/reference/auth
  type: oauth2
- description: Session cookie accepted for browser-originated (web app) requests, offered as an alternative to bearerAuth on every operation.
  in: cookie
  name: cookieAuth
  sources:
  - openapi/amika-openapi.json
  type: apiKey
slug: amika-authentication
source_filename: amika-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://docs.amika.dev/reference/auth.md\ndocs: https://docs.amika.dev/reference/auth\nsummary:\n  types: [http, apiKey, oauth2]\n  http_schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: [deviceAuthorization]\n  notes: >-\n    The OpenAPI declares two security requirements per operation (bearerAuth and\n    cookieAuth) but does not define them under components.securitySchemes. The\n    profile below is reconstructed from the published authentication docs.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer token in the Authorization header. The token is either a long-lived\n    API key created in the web UI (app.amika.dev/settings) or a short-lived\n    access token minted by the OAuth device-authorization login flow. The CLI\n    resolves credentials in precedence order: AMIKA_API_KEY env var, stored API\n    key file (${XDG_STATE_HOME}/amika/api-key.json), then browser login\
  \ session.\n  sources: [https://docs.amika.dev/reference/auth]\n- name: apiKey\n  type: apiKey\n  in: header\n  description: >-\n    API keys generated in the web UI for non-interactive/CI use. Provided via\n    the AMIKA_API_KEY environment variable or on-disk key file, presented as a\n    bearer token to the API. Managed through the /api-keys operations.\n  sources: [https://docs.amika.dev/reference/auth]\n- name: deviceAuthorization\n  type: oauth2\n  flow: deviceAuthorization\n  description: >-\n    Interactive browser login for local development. The CLI requests a device\n    code, the user authorizes in the browser, the CLI polls until complete, and\n    a session is stored with access token, refresh token, email, and org.\n    Tokens auto-refresh within 60 seconds of expiry. Identity is brokered by\n    WorkOS.\n  sources: [https://docs.amika.dev/reference/auth]\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  description: >-\n    Session cookie accepted for browser-originated\
  \ (web app) requests, offered\n    as an alternative to bearerAuth on every operation.\n  sources: [openapi/amika-openapi.json]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amika/refs/heads/main/authentication/amika-authentication.yml
summary_line: http/apiKey/oauth2 · 4 schemes
tags:
- Company
- AI Agents
- Coding Agents
- Developer Tools
- Sandboxes
- Infrastructure
- CI/CD
- Automation
- Software Factory
- API
---
