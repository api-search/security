---
api_key_in: []
api_specs:
- filename: streamlit-cloud-openapi.yml
  format: yaml
  label: Streamlit Community Cloud API
  slug: streamlit-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/streamlit/refs/heads/main/openapi/streamlit-cloud-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Streamlit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Streamlit secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Streamlit
provider_slug: streamlit
scheme_count: 1
schemes:
- description: 'Bearer token issued from the Streamlit Community Cloud account settings. Include as Authorization: Bearer {token}.'
  name: streamlitBearerAuth
  scheme: bearer
  sources:
  - openapi/streamlit-cloud-openapi.yml
  type: http
slug: streamlit-authentication
source_filename: streamlit-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/streamlit-cloud-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: streamlitBearerAuth\n  type: http\n  scheme: bearer\n  description: 'Bearer token issued from the Streamlit Community Cloud account settings. Include\n    as Authorization: Bearer {token}.'\n  sources:\n  - openapi/streamlit-cloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/streamlit/refs/heads/main/authentication/streamlit-authentication.yml
summary_line: http · 1 scheme
tags:
- Data Science
- Machine Learning
- Open Source
- Python
- Web Applications
---
