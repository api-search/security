---
anonymous_access: false
api_key_in: []
api_specs:
- filename: loadoptimizer-ai-health-api-openapi.yml
  format: yaml
  label: LoadOptimizer.ai Health API
  slug: loadoptimizer-ai-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loadoptimizer-ai/refs/heads/main/openapi/loadoptimizer-ai-health-api-openapi.yml
- filename: loadoptimizer-ai-jobs-api-openapi.yml
  format: yaml
  label: LoadOptimizer.ai Jobs API
  slug: loadoptimizer-ai-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/loadoptimizer-ai/refs/heads/main/openapi/loadoptimizer-ai-jobs-api-openapi.yml
auth_types: []
description: LoadOptimizer.ai uses a simple API key authentication scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Loadoptimizer Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: LoadOptimizer.ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LoadOptimizer.ai
provider_slug: loadoptimizer-ai
scheme_count: 1
schemes:
- evidence: 'Send the key on every request as the X-Api-Key header:'
  header: X-Api-Key
  how_to_obtain: Create the key in the web app; the full key is shown once immediately after creation.
  location: header
  name: X-Api-Key
  type: apiKey
slug: loadoptimizer-ai-authentication
source_filename: loadoptimizer-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.loadoptimizer.ai/docs/authentication.html
source_yaml: "generated: '2026-10-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.loadoptimizer.ai/docs/authentication.html\nsources:\n- https://www.loadoptimizer.ai/docs/authentication.html\n- https://www.loadoptimizer.ai/docs/quickstart.html\ndescription: LoadOptimizer.ai uses a simple API key authentication scheme.\nschemes:\n- type: apiKey\n  name: X-Api-Key\n  evidence: 'Send the key on every request as the X-Api-Key header:'\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Create the key in the web app; the full key is shown once immediately after creation.\nnote: No OAuth2, HTTP Bearer, HTTP Basic, JWT, HMAC, mTLS, or other authentication methods are documented.\ndocs: https://www.loadoptimizer.ai/docs/authentication.html\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/loadoptimizer-ai/refs/heads/main/authentication/loadoptimizer-ai-authentication.yml
summary_line: 1 scheme
tags:
- Logistics
- Artificial Intelligence
- Load Planning
- Optimization
- Shipping
---
