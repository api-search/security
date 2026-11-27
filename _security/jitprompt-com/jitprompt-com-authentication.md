---
anonymous_access: false
api_key_in: []
api_specs:
- filename: jitprompt-com-account-api-openapi.yml
  format: yaml
  label: jitprompt Account API
  slug: jitprompt-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jitprompt-com/openapi/jitprompt-com-account-api-openapi.yml
- filename: jitprompt-com-documents-api-openapi.yml
  format: yaml
  label: jitprompt Documents API
  slug: jitprompt-com-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jitprompt-com/openapi/jitprompt-com-documents-api-openapi.yml
- filename: jitprompt-com-pinned-documents-api-openapi.yml
  format: yaml
  label: jitprompt Pinned documents API
  slug: jitprompt-com-pinned-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jitprompt-com/openapi/jitprompt-com-pinned-documents-api-openapi.yml
- filename: jitprompt-com-versions-api-openapi.yml
  format: yaml
  label: jitprompt Versions API
  slug: jitprompt-com-versions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/jitprompt-com/openapi/jitprompt-com-versions-api-openapi.yml
auth_types: []
description: Authentication uses an API key provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: jitprompt Authentication
name_suffix: Authentication
oauth_flows: []
overview: jitprompt declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: jitprompt
provider_slug: jitprompt-com
scheme_count: 1
schemes:
- evidence: 'claude mcp add --transport http jitprompt-support-bot https://app.jitprompt.com/mcp \  --header "Authorization: Bearer imcp_..."'
  header: Authorization
  how_to_obtain: Create an API key in the namespace’s API keys page; the key is shown once and can be copied.
  location: header
  name: Bearer
  type: http-bearer
slug: jitprompt-com-authentication
source_filename: jitprompt-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.jitprompt.com/getting-started/introduction.md
source_yaml: "generated: '2026-11-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.jitprompt.com/getting-started/introduction.md\nsources:\n- https://docs.jitprompt.com/getting-started/introduction.md\n- https://docs.jitprompt.com/getting-started/quickstart.md\n- https://docs.jitprompt.com/getting-started/quickstart/\n- https://docs.jitprompt.com/getting-started/introduction/\ndescription: Authentication uses an API key provided as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'claude mcp add --transport http jitprompt-support-bot https://app.jitprompt.com/mcp \\  --header \"Authorization: Bearer imcp_...\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the namespace’s API keys page; the key is shown once and can be copied.\ndocs: https://docs.jitprompt.com/getting-started/introduction.md\n"
source_yaml_url: https://artifacts.apis.io/jitprompt-com/authentication/jitprompt-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
