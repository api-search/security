---
anonymous_access: false
api_key_in: []
auth_types: []
description: All API requests require an API key.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Localimpact Authentication
name_suffix: Authentication
oauth_flows: []
overview: LocalImpact declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LocalImpact
provider_slug: localimpact
scheme_count: 1
schemes:
- evidence: 'Pass your API key as a Bearer token:

    Authorization: Bearer YOUR_API_KEY'
  header: Authorization
  how_to_obtain: 'Generate an API key from: Account Management → Integrations → LocalImpact API'
  location: header
  name: Bearer
  type: http-bearer
slug: localimpact-authentication
source_filename: localimpact-authentication.yml
source_heading: Authentication Profile
source_url: https://localimpact.com/api#/#authentication
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://localimpact.com/api#/#authentication\nsources:\n- https://localimpact.com/api#/#authentication\n- https://localimpact.com/api#/\n- https://localimpact.com/api#/#getting-started\ndescription: All API requests require an API key.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Pass your API key as a Bearer token:\n\n    Authorization: Bearer YOUR_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Generate an API key from: Account Management → Integrations → LocalImpact API'\ndocs: https://localimpact.com/api#/#authentication\n"
source_yaml_url: https://artifacts.apis.io/localimpact/authentication/localimpact-authentication.yml
summary_line: 1 scheme
tags:
- Review
- Software-as-a-Service
- Local Business
- Reputation
- Software
---
