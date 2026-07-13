---
api_key_in:
- query
api_specs:
- filename: new-york-public-library-whats-on-the-menu-openapi-original.yaml
  format: yaml
  label: NYPL What's On The Menu API
  slug: new-york-public-library-whats-on-the-menu
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/new-york-public-library-whats-on-the-menu/refs/heads/main/openapi/new-york-public-library-whats-on-the-menu-openapi-original.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: New York Public Library Whats On The Menu Authentication
name_suffix: Authentication
oauth_flows: []
overview: New York Public Library What's On The Menu secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: New York Public Library What's On The Menu
provider_slug: new-york-public-library-whats-on-the-menu
scheme_count: 1
schemes:
- description: 26-character API token. Request access by emailing menus@nypl.org with subject "API ACCESS".
  in: query
  name: apiToken
  parameter: token
  sources:
  - openapi/new-york-public-library-whats-on-the-menu-openapi-original.yaml
  type: apiKey
slug: new-york-public-library-whats-on-the-menu-authentication
source_filename: new-york-public-library-whats-on-the-menu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/new-york-public-library-whats-on-the-menu-openapi-original.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiToken\n  type: apiKey\n  in: query\n  parameter: token\n  description: 26-character API token. Request access by emailing menus@nypl.org with subject\n    \"API ACCESS\".\n  sources:\n  - openapi/new-york-public-library-whats-on-the-menu-openapi-original.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/new-york-public-library-whats-on-the-menu/refs/heads/main/authentication/new-york-public-library-whats-on-the-menu-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Libraries
- Menus
- Restaurants
- History
- Open Data
- Food
- Datasets
- Cultural Heritage
---
