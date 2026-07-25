---
api_key_in: []
api_specs:
- filename: searchstax-authentication-api-openapi.yml
  format: yaml
  label: SearchStax Authentication API
  slug: searchstax-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchstax/refs/heads/main/openapi/searchstax-authentication-api-openapi.yml
- filename: searchstax-backup-api-openapi.yml
  format: yaml
  label: SearchStax Backup API
  slug: searchstax-backup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchstax/refs/heads/main/openapi/searchstax-backup-api-openapi.yml
- filename: searchstax-deployments-api-openapi.yml
  format: yaml
  label: SearchStax Deployments API
  slug: searchstax-deployments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchstax/refs/heads/main/openapi/searchstax-deployments-api-openapi.yml
- filename: searchstax-nodes-api-openapi.yml
  format: yaml
  label: SearchStax Nodes API
  slug: searchstax-nodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchstax/refs/heads/main/openapi/searchstax-nodes-api-openapi.yml
- filename: searchstax-plans-api-openapi.yml
  format: yaml
  label: SearchStax Plans API
  slug: searchstax-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchstax/refs/heads/main/openapi/searchstax-plans-api-openapi.yml
- filename: searchstax-usage-api-openapi.yml
  format: yaml
  label: SearchStax Usage API
  slug: searchstax-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/searchstax/refs/heads/main/openapi/searchstax-usage-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Searchstax Authentication
name_suffix: Authentication
oauth_flows: []
overview: SearchStax secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SearchStax
provider_slug: searchstax
scheme_count: 1
schemes:
- description: Token obtained from /obtain-auth-token/ endpoint
  name: tokenAuth
  scheme: bearer
  sources:
  - openapi/searchstax-provisioning-openapi.yml
  type: http
slug: searchstax-authentication
source_filename: searchstax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/searchstax-provisioning-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: tokenAuth\n  type: http\n  scheme: bearer\n  description: Token obtained from /obtain-auth-token/ endpoint\n  sources:\n  - openapi/searchstax-provisioning-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/searchstax/refs/heads/main/authentication/searchstax-authentication.yml
summary_line: http · 1 scheme
tags:
- Search
- Solr
- Managed Search
- Search Infrastructure
- Full-Text Search
- Site Search
---
