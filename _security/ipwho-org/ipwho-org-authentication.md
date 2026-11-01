---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ipwho-org-openapi-generated.yml
  format: yaml
  label: IPWho.org API
  slug: ipwho-org-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipwho-org/openapi/_ae-authored/ipwho-org-openapi-generated.yml
auth_types: []
description: Authentication is performed by providing an API key as a query parameter.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ipwho Org Authentication
name_suffix: Authentication
oauth_flows: []
overview: IPWho.org declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: IPWho.org
provider_slug: ipwho-org
scheme_count: 1
schemes:
- evidence: Terminal window curl " https://api.ipwho.org/ip/76.102.11.203?apiKey=sk.xxx "
  location: query
  name: apiKey
  type: apiKey
slug: ipwho-org-authentication
source_filename: ipwho-org-authentication.yml
source_heading: Authentication Profile
source_url: https://www.ipwho.org/docs/gettingstarted/overview
source_yaml: "generated: '2026-10-22'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.ipwho.org/docs/gettingstarted/overview\nsources:\n- https://www.ipwho.org/docs/gettingstarted/overview\ndescription: Authentication is performed by providing an API key as a query parameter.\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: Terminal window curl \" https://api.ipwho.org/ip/76.102.11.203?apiKey=sk.xxx \"\n  location: query\ndocs: https://www.ipwho.org/docs/gettingstarted/overview\n"
source_yaml_url: https://artifacts.apis.io/ipwho-org/authentication/ipwho-org-authentication.yml
summary_line: 1 scheme
tags:
- Company
- IP Geolocation
- Developer-Friendly
- Free Tier
---
