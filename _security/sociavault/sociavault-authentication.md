---
anonymous_access: false
api_key_in: []
auth_types: []
description: All API requests require authentication using your API key in the `X-API-Key` header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sociavault Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ziddec declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ziddec
provider_slug: sociavault
scheme_count: 1
schemes:
- evidence: All API requests require authentication using your API key in the `X-API-Key` header.
  header: X-API-Key
  how_to_obtain: Sign up at https://sociavault.com, navigate to your Dashboard, and copy your API key (starts with `sk_live_`).
  location: header
  name: API Key
  type: apiKey
slug: sociavault-authentication
source_filename: sociavault-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.sociavault.com/development.md
source_yaml: "generated: '2026-10-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.sociavault.com/development.md\nsources:\n- https://docs.sociavault.com/development.md\n- https://docs.sociavault.com/quickstart.md\ndescription: All API requests require authentication using your API key in the `X-API-Key` header.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: All API requests require authentication using your API key in the `X-API-Key` header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Sign up at https://sociavault.com, navigate to your Dashboard, and copy your API key (starts with `sk_live_`).\ndocs: https://docs.sociavault.com/development.md\n"
source_yaml_url: https://artifacts.apis.io/sociavault/authentication/sociavault-authentication.yml
summary_line: 1 scheme
tags:
- social-media-data
- Web Scraping
- Analytics
---
