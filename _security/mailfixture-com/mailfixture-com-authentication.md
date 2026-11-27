---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mailfixture-com-domains-api-openapi.yml
  format: yaml
  label: mailfixture Domains API
  slug: mailfixture-com-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-domains-api-openapi.yml
- filename: mailfixture-com-hooks-api-openapi.yml
  format: yaml
  label: mailfixture Hooks API
  slug: mailfixture-com-hooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-hooks-api-openapi.yml
- filename: mailfixture-com-inboxes-api-openapi.yml
  format: yaml
  label: mailfixture Inboxes API
  slug: mailfixture-com-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-inboxes-api-openapi.yml
- filename: mailfixture-com-keys-api-openapi.yml
  format: yaml
  label: mailfixture Keys API
  slug: mailfixture-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-keys-api-openapi.yml
- filename: mailfixture-com-messages-api-openapi.yml
  format: yaml
  label: mailfixture Messages API
  slug: mailfixture-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-messages-api-openapi.yml
- filename: mailfixture-com-phone-numbers-api-openapi.yml
  format: yaml
  label: mailfixture Phone Numbers API
  slug: mailfixture-com-phone-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-phone-numbers-api-openapi.yml
- filename: mailfixture-com-sms-api-openapi.yml
  format: yaml
  label: mailfixture Sms API
  slug: mailfixture-com-sms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-sms-api-openapi.yml
- filename: mailfixture-com-webhooks-api-openapi.yml
  format: yaml
  label: mailfixture Webhooks API
  slug: mailfixture-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mailfixture-com/openapi/mailfixture-com-webhooks-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: mailfixture Authentication
name_suffix: Authentication
oauth_flows: []
overview: mailfixture declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mailfixture
provider_slug: mailfixture-com
scheme_count: 1
schemes:
- evidence: Every request carries your key as a bearer token; create keys in Dashboard → API keys .
  header: Authorization
  how_to_obtain: Create keys in Dashboard → API keys
  location: header
  name: Bearer
  type: http-bearer
slug: mailfixture-com-authentication
source_filename: mailfixture-com-authentication.yml
source_heading: Authentication Profile
source_url: https://mailfixture.com/docs/api#auth
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mailfixture.com/docs/api#auth\nsources:\n- https://mailfixture.com/docs/api#auth\n- https://mailfixture.com/guides/email-auth-testing\n- https://mailfixture.com/docs/api\n- https://mailfixture.com/docs\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Every request carries your key as a bearer token; create keys in Dashboard → API keys .\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys in Dashboard → API keys\ndocs: https://mailfixture.com/docs/api#auth\n"
source_yaml_url: https://artifacts.apis.io/mailfixture-com/authentication/mailfixture-com-authentication.yml
summary_line: 1 scheme
tags:
- Email
- Testing
- Developer Tools
- Automation
---
