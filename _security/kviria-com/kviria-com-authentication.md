---
anonymous_access: false
api_key_in: []
api_specs:
- filename: kviria-com-account-api-openapi.yml
  format: yaml
  label: Kviria Account API
  slug: kviria-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kviria-com/openapi/kviria-com-account-api-openapi.yml
- filename: kviria-com-agent-api-openapi.yml
  format: yaml
  label: Kviria Agent API
  slug: kviria-com-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kviria-com/openapi/kviria-com-agent-api-openapi.yml
- filename: kviria-com-healthz-api-openapi.yml
  format: yaml
  label: Kviria Healthz API
  slug: kviria-com-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kviria-com/openapi/kviria-com-healthz-api-openapi.yml
auth_types: []
description: Authentication methods for Kviria API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Kviria Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kviria declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Kviria
provider_slug: kviria-com
scheme_count: 2
schemes:
- evidence: Every call carries it in the `Authorization` header.
  header: Authorization
  how_to_obtain: Open https://api.kviria.com/key and create a key. It is shown once, so copy it.
  location: header
  name: API Key
  type: http-bearer
- evidence: 'An MCP client can connect with OAuth instead: see Connect and pay.'
  name: MCP OAuth
  type: oauth2
slug: kviria-com-authentication
source_filename: kviria-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.kviria.com/quickstart.md
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.kviria.com/quickstart.md\nsources:\n- https://docs.kviria.com/quickstart.md\ndescription: Authentication methods for Kviria API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Every call carries it in the `Authorization` header.\n  location: header\n  header: Authorization\n  how_to_obtain: Open https://api.kviria.com/key and create a key. It is shown once, so copy it.\n- type: oauth2\n  name: MCP OAuth\n  evidence: 'An MCP client can connect with OAuth instead: see Connect and pay.'\ndocs: https://docs.kviria.com/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/kviria-com/authentication/kviria-com-authentication.yml
summary_line: 2 schemes
tags:
- location understanding
- AI Agents
- Privacy
---
