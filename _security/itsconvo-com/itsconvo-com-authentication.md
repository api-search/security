---
anonymous_access: false
api_key_in: []
api_specs:
- filename: itsconvo-com-ai-generation-api-openapi.yml
  format: yaml
  label: Convo AI Generation API
  slug: itsconvo-com-ai-generation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itsconvo-com/openapi/itsconvo-com-ai-generation-api-openapi.yml
- filename: itsconvo-com-calendar-api-openapi.yml
  format: yaml
  label: Convo Calendar API
  slug: itsconvo-com-calendar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itsconvo-com/openapi/itsconvo-com-calendar-api-openapi.yml
- filename: itsconvo-com-contacts-api-openapi.yml
  format: yaml
  label: Convo Contacts API
  slug: itsconvo-com-contacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itsconvo-com/openapi/itsconvo-com-contacts-api-openapi.yml
- filename: itsconvo-com-conversations-api-openapi.yml
  format: yaml
  label: Convo Conversations API
  slug: itsconvo-com-conversations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itsconvo-com/openapi/itsconvo-com-conversations-api-openapi.yml
- filename: itsconvo-com-user-api-openapi.yml
  format: yaml
  label: Convo User API
  slug: itsconvo-com-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itsconvo-com/openapi/itsconvo-com-user-api-openapi.yml
- filename: itsconvo-com-webhooks-api-openapi.yml
  format: yaml
  label: Convo Webhooks API
  slug: itsconvo-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/itsconvo-com/openapi/itsconvo-com-webhooks-api-openapi.yml
auth_types: []
description: Authentication uses an API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Convo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Convo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Convo
provider_slug: itsconvo-com
scheme_count: 1
schemes:
- evidence: Every request needs an API key in the `Authorization` header.
  header: Authorization
  how_to_obtain: Open the Convo desktop app and go to Settings → Convo API. Click Create key, give the key a name and accept the API Terms of Use.
  location: header
  name: API Key
  type: apiKey
slug: itsconvo-com-authentication
source_filename: itsconvo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.itsconvo.com/authentication.mdx
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.itsconvo.com/authentication.mdx\nsources:\n- https://docs.itsconvo.com/authentication.mdx\n- https://docs.itsconvo.com/authentication\n- https://docs.itsconvo.com/index.mdx\n- https://www.itsconvo.com/help-center/first-meeting-setup\ndescription: Authentication uses an API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Every request needs an API key in the `Authorization` header.\n  location: header\n  header: Authorization\n  how_to_obtain: Open the Convo desktop app and go to Settings → Convo API. Click Create key, give the key a name and accept the API Terms of\n    Use.\nnote: No OAuth2, http-bearer, http-basic, jwt, hmac, mtls, or other schemes are documented.\ndocs: https://docs.itsconvo.com/authentication.mdx\n"
source_yaml_url: https://artifacts.apis.io/itsconvo-com/authentication/itsconvo-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Sales
- Coaching
- Real-Time
---
