---
anonymous_access: false
api_key_in: []
api_specs:
- filename: trymnemo-com-namespace-api-openapi.yml
  format: yaml
  label: Mnemo Protocol Namespace API
  slug: trymnemo-com-namespace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymnemo-com/openapi/trymnemo-com-namespace-api-openapi.yml
- filename: trymnemo-com-objects-api-openapi.yml
  format: yaml
  label: Mnemo Protocol Objects API
  slug: trymnemo-com-objects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/trymnemo-com/openapi/trymnemo-com-objects-api-openapi.yml
auth_types: []
description: Authentication schemes for Mnemo Protocol
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mnemo Protocol Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mnemo Protocol declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Mnemo Protocol
provider_slug: trymnemo-com
scheme_count: 2
schemes:
- evidence: MnemoClient(api_key=...) sends the key in the X-API-Key header on every request to https://api.trymnemo.com .
  header: X-API-Key
  how_to_obtain: Get an API key from the Mnemo dashboard after signing in; the key is shown once.
  location: header
  name: X-API-Key
  type: apiKey
- evidence: 'Treat it as a secret: every later call authenticates with it.'
  header: X-Mnemo-Capability
  how_to_obtain: Create an ephemeral namespace via POST /v1/agent/namespaces; the response includes a one‑time capability.
  location: header
  name: X-Mnemo-Capability
  type: apiKey
slug: trymnemo-com-authentication
source_filename: trymnemo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.trymnemo.com/agents
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.trymnemo.com/agents\nsources:\n- https://www.trymnemo.com/agents\n- https://www.trymnemo.com/examples/agent-quickstart.sh\n- https://www.trymnemo.com/examples/agent_quickstart.py\n- https://www.trymnemo.com/docs/sdk\ndescription: Authentication schemes for Mnemo Protocol\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: MnemoClient(api_key=...) sends the key in the X-API-Key header on every request to https://api.trymnemo.com .\n  location: header\n  header: X-API-Key\n  how_to_obtain: Get an API key from the Mnemo dashboard after signing in; the key is shown once.\n- type: apiKey\n  name: X-Mnemo-Capability\n  evidence: 'Treat it as a secret: every later call authenticates with it.'\n  location: header\n  header: X-Mnemo-Capability\n  how_to_obtain: Create an ephemeral namespace via POST /v1/agent/namespaces; the response includes a one‑time capability.\ndocs:\
  \ https://www.trymnemo.com/agents\n"
source_yaml_url: https://artifacts.apis.io/trymnemo-com/authentication/trymnemo-com-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Embeddings
- Verification
- Vector Provenance
- Payments
---
