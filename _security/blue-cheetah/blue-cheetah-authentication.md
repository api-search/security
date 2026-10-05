---
anonymous_access: false
api_key_in: []
api_specs:
- filename: blue-cheetah-blue-cheetah-api-api-openapi.yml
  format: yaml
  label: Blue Cheetah Blue Cheetah API
  slug: blue-cheetah-blue-cheetah-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-cheetah/refs/heads/main/openapi/blue-cheetah-blue-cheetah-api-api-openapi.yml
- filename: blue-cheetah-chat-api-openapi.yml
  format: yaml
  label: Blue Cheetah Chat API
  slug: blue-cheetah-chat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-cheetah/refs/heads/main/openapi/blue-cheetah-chat-api-openapi.yml
- filename: blue-cheetah-completions-api-openapi.yml
  format: yaml
  label: Blue Cheetah Completions API
  slug: blue-cheetah-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-cheetah/refs/heads/main/openapi/blue-cheetah-completions-api-openapi.yml
- filename: blue-cheetah-health-api-openapi.yml
  format: yaml
  label: Blue Cheetah Health API
  slug: blue-cheetah-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-cheetah/refs/heads/main/openapi/blue-cheetah-health-api-openapi.yml
- filename: blue-cheetah-install-api-openapi.yml
  format: yaml
  label: Blue Cheetah Install API
  slug: blue-cheetah-install-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-cheetah/refs/heads/main/openapi/blue-cheetah-install-api-openapi.yml
- filename: blue-cheetah-metrics-api-openapi.yml
  format: yaml
  label: Blue Cheetah Metrics API
  slug: blue-cheetah-metrics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-cheetah/refs/heads/main/openapi/blue-cheetah-metrics-api-openapi.yml
- filename: blue-cheetah-tt-pkg-key-api-openapi.yml
  format: yaml
  label: Blue Cheetah Tt Pkg Key API
  slug: blue-cheetah-tt-pkg-key-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/blue-cheetah/refs/heads/main/openapi/blue-cheetah-tt-pkg-key-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Blue Cheetah Authentication
name_suffix: Authentication
oauth_flows: []
overview: Blue Cheetah declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Blue Cheetah
provider_slug: blue-cheetah
scheme_count: 1
schemes:
- evidence: Your JWT_SECRET is used to create an API key for authenticating requests.
  header: Authorization
  how_to_obtain: Set JWT_SECRET environment variable and generate API key via provided script.
  location: header
  name: Bearer
  type: http-bearer
slug: blue-cheetah-authentication
source_filename: blue-cheetah-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.tenstorrent.com/getting-started/README.html
source_yaml: "generated: '2026-09-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.tenstorrent.com/getting-started/README.html\nsources:\n- https://docs.tenstorrent.com/getting-started/README.html\n- https://docs.tenstorrent.com/getting-started/vLLM-servers.html\n- https://docs.tenstorrent.com/getting-started/tt-software-stack.html\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Your JWT_SECRET is used to create an API key for authenticating requests.\n  location: header\n  header: Authorization\n  how_to_obtain: Set JWT_SECRET environment variable and generate API key via provided script.\nnote: No other authentication schemes are documented on the provided pages.\ndocs: https://docs.tenstorrent.com/getting-started/README.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/blue-cheetah/refs/heads/main/authentication/blue-cheetah-authentication.yml
summary_line: 1 scheme
tags:
- AI Hardware
- Compute
- Servers
- Workstations
---
