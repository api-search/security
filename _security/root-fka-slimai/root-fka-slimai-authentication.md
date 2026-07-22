---
api_key_in:
- header (Authorization)
api_specs:
- filename: root-fka-slimai-openapi-original.json
  format: json
  label: Root.io API
  slug: rootio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/root-fka-slimai/refs/heads/main/openapi/root-fka-slimai-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Root Fka Slimai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Root (fka Slim.ai) secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Root (fka Slim.ai)
provider_slug: root-fka-slimai
scheme_count: 2
schemes:
- detail: API key used as the Basic-auth username with an empty password. Declared as the BasicAuth securityDefinition in the OpenAPI.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/root-fka-slimai-openapi-original.json
  type: http
- detail: API key sent as a Bearer token in the Authorization header (documented in the API reference; not declared in the Swagger securityDefinitions).
  name: BearerToken
  scheme: bearer
  sources:
  - https://docs.root.io/reference/api
  type: http
slug: root-fka-slimai-authentication
source_filename: root-fka-slimai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.root.io/reference/api; https://docs.root.io/getting-started/authentication; openapi/root-fka-slimai-openapi-original.json\ndocs: https://docs.root.io/getting-started/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - basic\n  - bearer\n  api_key_in:\n  - header (Authorization)\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  detail: API key used as the Basic-auth username with an empty password. Declared as the BasicAuth securityDefinition\n    in the OpenAPI.\n  sources:\n  - openapi/root-fka-slimai-openapi-original.json\n- name: BearerToken\n  type: http\n  scheme: bearer\n  detail: API key sent as a Bearer token in the Authorization header (documented in the API reference;\n    not declared in the Swagger securityDefinitions).\n  sources:\n  - https://docs.root.io/reference/api\napi_keys:\n  management: Create/rotate API keys in the Root platform Settings -> API Keys; managed via\
  \ /v3/api_keys.\n  registry_tokens: Separate long-lived registry tokens (username rootio / org id) authenticate to cr.root.io\n    and pkg.root.io; rotatable from the platform.\nunauthenticated: Feed endpoints under /external/* (CVE feed, patch feed, OSV feed) and OSV records require\n  no auth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/root-fka-slimai/refs/heads/main/authentication/root-fka-slimai-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- Security
- Vulnerability Management
- Container Security
- DevSecOps
- Software Supply Chain
- CVE
- SBOM
- Open Source
- Patching
---
