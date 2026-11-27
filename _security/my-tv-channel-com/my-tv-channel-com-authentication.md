---
anonymous_access: false
api_key_in: []
api_specs:
- filename: my-tv-channel-com-account-api-openapi.yml
  format: yaml
  label: My TV Channel Account API
  slug: my-tv-channel-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/my-tv-channel-com/openapi/my-tv-channel-com-account-api-openapi.yml
- filename: my-tv-channel-com-channels-api-openapi.yml
  format: yaml
  label: My TV Channel Channels API
  slug: my-tv-channel-com-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/my-tv-channel-com/openapi/my-tv-channel-com-channels-api-openapi.yml
- filename: my-tv-channel-com-content-api-openapi.yml
  format: yaml
  label: My TV Channel Content API
  slug: my-tv-channel-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/my-tv-channel-com/openapi/my-tv-channel-com-content-api-openapi.yml
- filename: my-tv-channel-com-scheduling-api-openapi.yml
  format: yaml
  label: My TV Channel Scheduling API
  slug: my-tv-channel-com-scheduling-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/my-tv-channel-com/openapi/my-tv-channel-com-scheduling-api-openapi.yml
auth_types: []
description: Authentication for My TV Channel MCP API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: My TV Channel Authentication
name_suffix: Authentication
oauth_flows: []
overview: My TV Channel declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: My TV Channel
provider_slug: my-tv-channel-com
scheme_count: 1
schemes:
- evidence: '`Auth:` `Authorization: Bearer mytv_sk_...`'
  header: Authorization
  how_to_obtain: In the app under Profile → Agent Access, or at https://my-tv-channel.com/agent-keys/.
  location: header
  name: Bearer
  type: http-bearer
slug: my-tv-channel-com-authentication
source_filename: my-tv-channel-com-authentication.yml
source_heading: Authentication Profile
source_url: https://my-tv-channel.com/api/mytvchannel/mcp/README.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://my-tv-channel.com/api/mytvchannel/mcp/README.md\nsources:\n- https://my-tv-channel.com/api/mytvchannel/mcp/README.md\ndescription: Authentication for My TV Channel MCP API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: '`Auth:` `Authorization: Bearer mytv_sk_...`'\n  location: header\n  header: Authorization\n  how_to_obtain: In the app under Profile → Agent Access, or at https://my-tv-channel.com/agent-keys/.\ndocs: https://my-tv-channel.com/api/mytvchannel/mcp/README.md\n"
source_yaml_url: https://artifacts.apis.io/my-tv-channel-com/authentication/my-tv-channel-com-authentication.yml
summary_line: 1 scheme
tags:
- Media
- Streaming
- Video
- Platform
- Creators
---
