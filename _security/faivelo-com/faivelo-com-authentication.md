---
anonymous_access: false
api_key_in: []
api_specs:
- filename: faivelo-com-core-openapi-generated.yml
  format: yaml
  label: Faivelo core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faivelo-com/openapi/_ae-authored/faivelo-com-core-openapi-generated.yml
- filename: faivelo-com-transactional-openapi-generated.yml
  format: yaml
  label: Faivelo transactional API
  slug: transactional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faivelo-com/openapi/_ae-authored/faivelo-com-transactional-openapi-generated.yml
- filename: faivelo-com-v1-openapi-generated.yml
  format: yaml
  label: Faivelo v1 API
  slug: v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/faivelo-com/openapi/_ae-authored/faivelo-com-v1-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Faivelo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Faivelo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Faivelo
provider_slug: faivelo-com
scheme_count: 1
schemes:
- evidence: 'Authenticate with a Bearer header: curl https://faivelo.com/api/v1/mailboxes \ -H "Authorization: Bearer fvl_live_..."'
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: faivelo-com-authentication
source_filename: faivelo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://faivelo.com/docs/developers/ai-agents
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://faivelo.com/docs/developers/ai-agents\nsources:\n- https://faivelo.com/docs/developers/ai-agents\n- https://faivelo.com/hosting/pocketbase\n- https://faivelo.com/hosting/node-red\n- https://faivelo.com/guides/cloudflare-email-setup\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authenticate with a Bearer header: curl https://faivelo.com/api/v1/mailboxes \\ -H \"Authorization: Bearer fvl_live_...\"'\n  location: header\n  header: Authorization\ndocs: https://faivelo.com/docs/developers/ai-agents\n"
source_yaml_url: https://artifacts.apis.io/faivelo-com/authentication/faivelo-com-authentication.yml
summary_line: 1 scheme
tags:
- Business Email
- Transactional Email
- Marketing Email
- Email API
- AI Agents
---
