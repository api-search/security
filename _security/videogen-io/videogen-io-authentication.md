---
anonymous_access: false
api_key_in: []
api_specs:
- filename: videogen-io-account-api-openapi.yml
  format: yaml
  label: VideoGen Account API
  slug: videogen-io-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-account-api-openapi.yml
- filename: videogen-io-assistant-api-openapi.yml
  format: yaml
  label: VideoGen Assistant API
  slug: videogen-io-assistant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-assistant-api-openapi.yml
- filename: videogen-io-entities-api-openapi.yml
  format: yaml
  label: VideoGen Entities API
  slug: videogen-io-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-entities-api-openapi.yml
- filename: videogen-io-files-api-openapi.yml
  format: yaml
  label: VideoGen Files API
  slug: videogen-io-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-files-api-openapi.yml
- filename: videogen-io-projects-api-openapi.yml
  format: yaml
  label: VideoGen Projects API
  slug: videogen-io-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-projects-api-openapi.yml
- filename: videogen-io-resources-api-openapi.yml
  format: yaml
  label: VideoGen Resources API
  slug: videogen-io-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-resources-api-openapi.yml
- filename: videogen-io-text-api-openapi.yml
  format: yaml
  label: VideoGen Text API
  slug: videogen-io-text-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-text-api-openapi.yml
- filename: videogen-io-tools-api-openapi.yml
  format: yaml
  label: VideoGen Tools API
  slug: videogen-io-tools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-tools-api-openapi.yml
- filename: videogen-io-webhook-events-api-openapi.yml
  format: yaml
  label: VideoGen Webhook events API
  slug: videogen-io-webhook-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-webhook-events-api-openapi.yml
- filename: videogen-io-webhooks-api-openapi.yml
  format: yaml
  label: VideoGen Webhooks API
  slug: videogen-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-webhooks-api-openapi.yml
- filename: videogen-io-workflows-api-openapi.yml
  format: yaml
  label: VideoGen Workflows API
  slug: videogen-io-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/openapi/videogen-io-workflows-api-openapi.yml
auth_types: []
description: Authentication methods for VideoGen API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Videogen Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: VideoGen declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: VideoGen
provider_slug: videogen-io
scheme_count: 2
schemes:
- evidence: Create an API key from the VideoGen dashboard, set the Authorization bearer header, and keep credentials safe with environment variables.
  header: Authorization
  how_to_obtain: Create a key in the VideoGen dashboard at https://app.videogen.io/api, copy the displayed key, and store it securely.
  location: header
  name: API key
  type: http-bearer
- authorize_url: '{authorization_endpoint}'
  evidence: Use OAuth 2.1 (authorization code with PKCE) to let users authorize your application to call the VideoGen API on their behalf.
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Register your application via the developer dashboard at https://app.videogen.io/api to receive a client_id (and client_secret for confidential clients). Then follow the authorization code flow with PKCE as described.
  location: header
  name: OAuth 2.1
  scopes:
  - email
  - profile
  - openid
  type: oauth2
slug: videogen-io-authentication
source_filename: videogen-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.videogen.io/authentication.md
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.videogen.io/authentication.md\nsources:\n- https://docs.videogen.io/authentication.md\n- https://docs.videogen.io/oauth.md\n- https://docs.videogen.io/getting-started.md\n- https://help.videogen.io/en/collections/14592492-getting-started\ndescription: Authentication methods for VideoGen API\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: Create an API key from the VideoGen dashboard, set the Authorization bearer header, and keep credentials safe with environment variables.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the VideoGen dashboard at https://app.videogen.io/api, copy the displayed key, and store it securely.\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Use OAuth 2.1 (authorization code with PKCE) to let users authorize your application to call the VideoGen API on their behalf.\n  location: header\n  header:\
  \ Authorization\n  flows:\n  - authorization_code\n  authorize_url: '{authorization_endpoint}'\n  scopes:\n  - email\n  - profile\n  - openid\n  how_to_obtain: Register your application via the developer dashboard at https://app.videogen.io/api to receive a client_id (and client_secret\n    for confidential clients). Then follow the authorization code flow with PKCE as described.\ndocs: https://docs.videogen.io/authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/videogen-io/refs/heads/main/authentication/videogen-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Video
- Automation
- Platform
---
