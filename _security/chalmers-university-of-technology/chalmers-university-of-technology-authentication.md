---
api_key_in: []
api_specs:
- filename: chalmers-university-of-technology-research-api.yaml
  format: yaml
  label: Chalmers Research API
  slug: research-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chalmers-university-of-technology/refs/heads/main/openapi/chalmers-university-of-technology-research-api.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Chalmers University Of Technology Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chalmers University of Technology secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Chalmers University of Technology
provider_slug: chalmers-university-of-technology
scheme_count: 1
schemes:
- description: Basic HTTP Authentication
  name: basic
  scheme: basic
  sources:
  - openapi/chalmers-university-of-technology-research-api.yaml
  type: http
slug: chalmers-university-of-technology-authentication
source_filename: chalmers-university-of-technology-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/chalmers-university-of-technology-research-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: basic\n  type: http\n  scheme: basic\n  description: Basic HTTP Authentication\n  sources:\n  - openapi/chalmers-university-of-technology-research-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chalmers-university-of-technology/refs/heads/main/authentication/chalmers-university-of-technology-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- Higher Education
- University
- Research
- Open Data
- Library
- OAI-PMH
- Sweden
---
