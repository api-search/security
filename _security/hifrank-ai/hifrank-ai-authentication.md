---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hifrank-ai-openapi-generated.yml
  format: yaml
  label: Frank API
  slug: hifrank-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hifrank-ai/openapi/_ae-authored/hifrank-ai-openapi-generated.yml
auth_types: []
description: Authentication schemes for Frank
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hifrank Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Frank declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Frank
provider_slug: hifrank-ai
scheme_count: 1
schemes:
- evidence: Every request carries your secret — a frank_whsec_‑prefixed value — in the X-Frank-Signature header.
  header: X-Frank-Signature
  how_to_obtain: Generated in Frank webhook settings and displayed (masked) in the Signing secret field; rotate to get a new value.
  location: header
  name: Signing secret
  type: apiKey
slug: hifrank-ai-authentication
source_filename: hifrank-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.hifrank.ai/docs/set-up-the-frank-webhook
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.hifrank.ai/docs/set-up-the-frank-webhook\nsources:\n- https://www.hifrank.ai/docs/set-up-the-frank-webhook\n- https://www.hifrank.ai/docs/how-to-set-it-up\n- https://www.hifrank.ai/docs/how-to-create-a-new-product\ndescription: Authentication schemes for Frank\nschemes:\n- type: apiKey\n  name: Signing secret\n  evidence: Every request carries your secret — a frank_whsec_‑prefixed value — in the X-Frank-Signature header.\n  location: header\n  header: X-Frank-Signature\n  how_to_obtain: Generated in Frank webhook settings and displayed (masked) in the Signing secret field; rotate to get a new value.\nnote: No OAuth2 or other authentication methods are documented on the provided pages.\ndocs: https://www.hifrank.ai/docs/set-up-the-frank-webhook\n"
source_yaml_url: https://artifacts.apis.io/hifrank-ai/authentication/hifrank-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Customer Research
- InterviewAutomation
- Market Insights
- Software-as-a-Service
---
