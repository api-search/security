---
api_key_in:
- query
api_specs:
- filename: university-of-warsaw-usos-api.yaml
  format: yaml
  label: USOS API (University of Warsaw)
  slug: usos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/openapi/university-of-warsaw-usos-api.yaml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: University Of Warsaw Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Warsaw secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Warsaw
provider_slug: university-of-warsaw
scheme_count: 1
schemes:
- description: USOS API uses OAuth 1.0a for authorized methods. A Consumer Key/Secret is obtained from the USOS developers portal (https://usosapps.uw.edu.pl/developers/), and an access token is obtained via the OAuth flow documented at https://usosapps.uw.edu.pl/developers/api/authorization/. The methods described in this file are anonymous and do not require it.
  in: query
  name: oauth1a
  parameter: oauth_token
  sources:
  - openapi/university-of-warsaw-usos-api.yaml
  type: apiKey
slug: university-of-warsaw-authentication
source_filename: university-of-warsaw-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-warsaw-usos-api.yaml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: oauth1a\n  type: apiKey\n  in: query\n  parameter: oauth_token\n  description: USOS API uses OAuth 1.0a for authorized methods. A Consumer Key/Secret is obtained\n    from the USOS developers portal (https://usosapps.uw.edu.pl/developers/), and an access\n    token is obtained via the OAuth flow documented at https://usosapps.uw.edu.pl/developers/api/authorization/.\n    The methods described in this file are anonymous and do not require it.\n  sources:\n  - openapi/university-of-warsaw-usos-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-warsaw/refs/heads/main/authentication/university-of-warsaw-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Education
- Higher Education
- University
- Poland
- Academic Data
- Research Data
- Open Data
---
