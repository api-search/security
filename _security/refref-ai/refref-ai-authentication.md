---
anonymous_access: false
api_key_in: []
api_specs:
- filename: refref-ai-openapi-generated.yml
  format: yaml
  label: RefRef API
  slug: refref-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/refref-ai/openapi/_ae-authored/refref-ai-openapi-generated.yml
auth_types: []
description: Authentication schemes for RefRef API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: RefRef Authentication
name_suffix: Authentication
oauth_flows: []
overview: RefRef declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: RefRef
provider_slug: refref-ai
scheme_count: 1
schemes:
- evidence: Your backend makes these calls with a Workspace API key in the X-Api-Key header.
  header: X-Api-Key
  how_to_obtain: Provided as a Workspace API key (e.g., REFREF_API_KEY) in the server environment.
  location: header
  name: Workspace API key
  type: apiKey
slug: refref-ai-authentication
source_filename: refref-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://refref.ai/docs/platform/better-auth
source_yaml: "generated: '2026-11-23'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://refref.ai/docs/platform/better-auth\nsources:\n- https://refref.ai/docs/platform/better-auth\n- https://refref.ai/docs/platform/installation/auth\n- https://refref.ai/blog/add-referral-program-stripe-better-auth\ndescription: Authentication schemes for RefRef API\nschemes:\n- type: apiKey\n  name: Workspace API key\n  evidence: Your backend makes these calls with a Workspace API key in the X-Api-Key header.\n  location: header\n  header: X-Api-Key\n  how_to_obtain: Provided as a Workspace API key (e.g., REFREF_API_KEY) in the server environment.\ndocs: https://refref.ai/docs/platform/better-auth\n"
source_yaml_url: https://artifacts.apis.io/refref-ai/authentication/refref-ai-authentication.yml
summary_line: 1 scheme
tags:
- Referral
- Affiliate
- Loyalty
- OpenSource
- SaaS
---
