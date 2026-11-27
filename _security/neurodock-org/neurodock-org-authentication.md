---
anonymous_access: false
api_key_in: []
api_specs:
- filename: neurodock-org-openapi-generated.yml
  format: yaml
  label: NeuroDock API
  slug: neurodock-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/neurodock-org/openapi/_ae-authored/neurodock-org-openapi-generated.yml
auth_types: []
description: OAuth 2.1 (PKCE) authentication for the hosted MCP endpoint.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: NeuroDock Authentication
name_suffix: Authentication
oauth_flows: []
overview: NeuroDock declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: NeuroDock
provider_slug: neurodock-org
scheme_count: 1
schemes:
- evidence: Transport is Streamable HTTP ; auth is OAuth 2.1 (PKCE).
  flows:
  - authorization_code
  name: OAuth 2.1 PKCE
  type: oauth2
slug: neurodock-org-authentication
source_filename: neurodock-org-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.neurodock.org/getting-started/im-tired/
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.neurodock.org/getting-started/im-tired/\nsources:\n- https://docs.neurodock.org/getting-started/im-tired/\n- https://docs.neurodock.org/getting-started/installation/\n- https://docs.neurodock.org/getting-started/remote/\n- https://docs.neurodock.org/getting-started/first-skill/\ndescription: OAuth 2.1 (PKCE) authentication for the hosted MCP endpoint.\nschemes:\n- type: oauth2\n  name: OAuth 2.1 PKCE\n  evidence: Transport is Streamable HTTP ; auth is OAuth 2.1 (PKCE).\n  flows:\n  - authorization_code\ndocs: https://docs.neurodock.org/getting-started/im-tired/\n"
source_yaml_url: https://artifacts.apis.io/neurodock-org/authentication/neurodock-org-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Neurodiversity
- Productivity
- Open Source
---
