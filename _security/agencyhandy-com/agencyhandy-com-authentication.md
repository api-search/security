---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods as published on Agency Handy documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Agency Handy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agency Handy declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Agency Handy
provider_slug: agencyhandy-com
scheme_count: 1
schemes:
- evidence: Every request is authenticated with an API key that you generate from your workspace settings.
  header: x-api-key
  how_to_obtain: Generate an API key in Workspace Configuration under the API Key tab.
  location: header
  name: API Key
  type: apiKey
slug: agencyhandy-com-authentication
source_filename: agencyhandy-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.agencyhandy.com/api/getting-started.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.agencyhandy.com/api/getting-started.md\nsources:\n- https://docs.agencyhandy.com/api/getting-started.md\n- https://docs.agencyhandy.com/getting-started/introduction.md\n- https://docs.agencyhandy.com/getting-started/sign-up.md\n- https://docs.agencyhandy.com/getting-started/log-in.md\ndescription: Authentication methods as published on Agency Handy documentation.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Every request is authenticated with an API key that you generate from your workspace settings.\n  location: header\n  header: x-api-key\n  how_to_obtain: Generate an API key in Workspace Configuration under the API Key tab.\nnote: All authenticated requests also require a `companyid` header, but it is not an authentication credential.\ndocs: https://docs.agencyhandy.com/api/getting-started.md\n"
source_yaml_url: https://artifacts.apis.io/agencyhandy-com/authentication/agencyhandy-com-authentication.yml
summary_line: 1 scheme
tags:
- Agency
- Software-as-a-Service
- Client Portal
- Project Management
- Invoicing
---
