---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ethora-com-agents-api-openapi.yml
  format: yaml
  label: Ethora Agents API
  slug: ethora-com-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-agents-api-openapi.yml
- filename: ethora-com-ai-widget-api-openapi.yml
  format: yaml
  label: Ethora AI Widget API
  slug: ethora-com-ai-widget-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-ai-widget-api-openapi.yml
- filename: ethora-com-apps-api-openapi.yml
  format: yaml
  label: Ethora Apps API
  slug: ethora-com-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-apps-api-openapi.yml
- filename: ethora-com-auth-api-openapi.yml
  format: yaml
  label: Ethora Auth API
  slug: ethora-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-auth-api-openapi.yml
- filename: ethora-com-chats-api-openapi.yml
  format: yaml
  label: Ethora Chats API
  slug: ethora-com-chats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-chats-api-openapi.yml
- filename: ethora-com-files-api-openapi.yml
  format: yaml
  label: Ethora Files API
  slug: ethora-com-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-files-api-openapi.yml
- filename: ethora-com-push-api-openapi.yml
  format: yaml
  label: Ethora Push API
  slug: ethora-com-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-push-api-openapi.yml
- filename: ethora-com-sharelinks-api-openapi.yml
  format: yaml
  label: Ethora Sharelinks API
  slug: ethora-com-sharelinks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-sharelinks-api-openapi.yml
- filename: ethora-com-users-api-openapi.yml
  format: yaml
  label: Ethora Users API
  slug: ethora-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ethora-com/openapi/ethora-com-users-api-openapi.yml
auth_types: []
description: Authentication uses JWT tokens passed in the Authorization header as a Bearer token, with a legacy fallback to the x‑custom‑token header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Ethora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ethora declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ethora
provider_slug: ethora-com
scheme_count: 2
schemes:
- evidence: 'Prefer Authorization: Bearer <JWT>; x-custom-token is still accepted for backward compatibility.'
  header: Authorization
  location: header
  name: Authorization
  type: http-bearer
- evidence: 'Prefer Authorization: Bearer <JWT>; x-custom-token is still accepted for backward compatibility.'
  header: x-custom-token
  location: header
  name: x-custom-token
  type: http-bearer
slug: ethora-com-authentication
source_filename: ethora-com-authentication.yml
source_heading: Authentication Profile
source_url: https://api.chat.ethora.com/api-docs/#/Auth
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.chat.ethora.com/api-docs/#/Auth\nsources:\n- https://api.chat.ethora.com/api-docs/#/Auth\ndescription: Authentication uses JWT tokens passed in the Authorization header as a Bearer token, with a legacy fallback to the x‑custom‑token\n  header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Prefer Authorization: Bearer <JWT>; x-custom-token is still accepted for backward compatibility.'\n  location: header\n  header: Authorization\n- type: http-bearer\n  name: x-custom-token\n  evidence: 'Prefer Authorization: Bearer <JWT>; x-custom-token is still accepted for backward compatibility.'\n  location: header\n  header: x-custom-token\ndocs: https://api.chat.ethora.com/api-docs/#/Auth\n"
source_yaml_url: https://artifacts.apis.io/ethora-com/authentication/ethora-com-authentication.yml
summary_line: 2 schemes
tags:
- Chat
- Artificial Intelligence
- SDK
- Low-Code
- Messaging
---
