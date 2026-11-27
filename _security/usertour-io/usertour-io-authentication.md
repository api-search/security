---
anonymous_access: false
api_key_in: []
api_specs:
- filename: usertour-io-analytics-api-openapi.yml
  format: yaml
  label: Usertour Analytics API
  slug: usertour-io-analytics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-analytics-api-openapi.yml
- filename: usertour-io-attribute-definitions-api-openapi.yml
  format: yaml
  label: Usertour Attribute definitions API
  slug: usertour-io-attribute-definitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-attribute-definitions-api-openapi.yml
- filename: usertour-io-companies-api-openapi.yml
  format: yaml
  label: Usertour Companies API
  slug: usertour-io-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-companies-api-openapi.yml
- filename: usertour-io-content-api-openapi.yml
  format: yaml
  label: Usertour Content API
  slug: usertour-io-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-content-api-openapi.yml
- filename: usertour-io-content-versions-api-openapi.yml
  format: yaml
  label: Usertour Content versions API
  slug: usertour-io-content-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-content-versions-api-openapi.yml
- filename: usertour-io-environments-api-openapi.yml
  format: yaml
  label: Usertour Environments API
  slug: usertour-io-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-environments-api-openapi.yml
- filename: usertour-io-event-definitions-api-openapi.yml
  format: yaml
  label: Usertour Event definitions API
  slug: usertour-io-event-definitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-event-definitions-api-openapi.yml
- filename: usertour-io-events-api-openapi.yml
  format: yaml
  label: Usertour Events API
  slug: usertour-io-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-events-api-openapi.yml
- filename: usertour-io-localizations-api-openapi.yml
  format: yaml
  label: Usertour Localizations API
  slug: usertour-io-localizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-localizations-api-openapi.yml
- filename: usertour-io-me-api-openapi.yml
  format: yaml
  label: Usertour Me API
  slug: usertour-io-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-me-api-openapi.yml
- filename: usertour-io-segments-api-openapi.yml
  format: yaml
  label: Usertour Segments API
  slug: usertour-io-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-segments-api-openapi.yml
- filename: usertour-io-sessions-api-openapi.yml
  format: yaml
  label: Usertour Sessions API
  slug: usertour-io-sessions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-sessions-api-openapi.yml
- filename: usertour-io-themes-api-openapi.yml
  format: yaml
  label: Usertour Themes API
  slug: usertour-io-themes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-themes-api-openapi.yml
- filename: usertour-io-users-api-openapi.yml
  format: yaml
  label: Usertour Users API
  slug: usertour-io-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-users-api-openapi.yml
- filename: usertour-io-webhooks-api-openapi.yml
  format: yaml
  label: Usertour Webhooks API
  slug: usertour-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usertour-io/openapi/usertour-io-webhooks-api-openapi.yml
auth_types: []
description: Usertour API v2 authenticates using personal API tokens sent as a Bearer header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Usertour Authentication
name_suffix: Authentication
oauth_flows: []
overview: Usertour declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Usertour
provider_slug: usertour-io
scheme_count: 1
schemes:
- evidence: 'The v2 API authenticates with **personal API tokens**. Create one in your Usertour dashboard under **Settings → Personal API keys**, then send it as a Bearer header on every request:'
  header: Authorization
  how_to_obtain: Create one in your Usertour dashboard under Settings → Personal API keys.
  location: header
  name: Personal API token
  scopes:
  - content:read
  - content:create
  - content:update
  - content:delete
  - content:publish
  - theme:read
  - theme:create
  - theme:update
  - theme:delete
  - localization:read
  - localization:create
  - localization:update
  - localization:delete
  - user:read
  - user:write
  - user:delete
  - company:read
  - company:write
  - company:delete
  - session:read
  - session:manage
  - attribute:read
  - attribute:create
  - attribute:update
  - attribute:delete
  - event:read
  - event:create
  - event:update
  - event:delete
  - segment:read
  - segment:create
  - segment:update
  - segment:delete
  - analytics:read
  - environment:read
  - environment:manage
  type: http-bearer
slug: usertour-io-authentication
source_filename: usertour-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.usertour.io/how-to-guides/two-factor-authentication.md
source_yaml: "generated: '2026-11-27'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.usertour.io/how-to-guides/two-factor-authentication.md\nsources:\n- https://docs.usertour.io/how-to-guides/two-factor-authentication.md\n- https://docs.usertour.io/api-reference-v2/authentication.md\n- https://docs.usertour.io/api-reference/webhooks/get-a-webhook-includes-the-signing-secret-for-webhook:manage-tokens.md\n- https://docs.usertour.io/api-reference/webhooks/rotate-the-signing-secret.md\ndescription: Usertour API v2 authenticates using personal API tokens sent as a Bearer header.\nschemes:\n- type: http-bearer\n  name: Personal API token\n  evidence: 'The v2 API authenticates with **personal API tokens**. Create one in your Usertour dashboard under **Settings → Personal API keys**,\n    then send it as a Bearer header on every request:'\n  location: header\n  header: Authorization\n  scopes:\n  - content:read\n  - content:create\n  - content:update\n  - content:delete\n\
  \  - content:publish\n  - theme:read\n  - theme:create\n  - theme:update\n  - theme:delete\n  - localization:read\n  - localization:create\n  - localization:update\n  - localization:delete\n  - user:read\n  - user:write\n  - user:delete\n  - company:read\n  - company:write\n  - company:delete\n  - session:read\n  - session:manage\n  - attribute:read\n  - attribute:create\n  - attribute:update\n  - attribute:delete\n  - event:read\n  - event:create\n  - event:update\n  - event:delete\n  - segment:read\n  - segment:create\n  - segment:update\n  - segment:delete\n  - analytics:read\n  - environment:read\n  - environment:manage\n  how_to_obtain: Create one in your Usertour dashboard under Settings → Personal API keys.\ndocs: https://docs.usertour.io/how-to-guides/two-factor-authentication.md\n"
source_yaml_url: https://artifacts.apis.io/usertour-io/authentication/usertour-io-authentication.yml
summary_line: 1 scheme
tags:
- Company
- OpenSource
- UserOnboarding
- SaaS
- DeveloperTools
---
