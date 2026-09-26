---
anonymous_access: false
api_key_in: []
api_specs:
- filename: janus-machine-market-search-github-ingress-openapi.yml
  format: yaml
  label: JANUS.SEARCH GitHub Issues Ingress
  slug: janus-search-github-ingress
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/janus-machine-market/refs/heads/main/openapi/janus-machine-market-search-github-ingress-openapi.yml
- filename: janus-machine-market-pr-review-github-ingress-openapi.yml
  format: yaml
  label: JANUS.PR_REVIEW GitHub Issues Ingress
  slug: janus-pr-review-github-ingress
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/janus-machine-market/refs/heads/main/openapi/janus-machine-market-pr-review-github-ingress-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Janus Machine Market Authentication
name_suffix: Authentication
oauth_flows: []
overview: JANUS Machine Market secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JANUS Machine Market
provider_slug: janus-machine-market
scheme_count: 1
schemes:
- description: Caller-supplied GitHub credential used only to create/read the Market issue.
  name: githubBearer
  scheme: bearer
  sources:
  - openapi/janus-machine-market-pr-review-github-ingress-openapi.yml
  - openapi/janus-machine-market-search-github-ingress-openapi.yml
  type: http
slug: janus-machine-market-authentication
source_filename: janus-machine-market-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: derived\nsource: openapi/janus-machine-market-pr-review-github-ingress-openapi.yml, openapi/janus-machine-market-search-github-ingress-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: githubBearer\n  type: http\n  scheme: bearer\n  description: Caller-supplied GitHub credential used only to create/read the Market issue.\n  sources:\n  - openapi/janus-machine-market-pr-review-github-ingress-openapi.yml\n  - openapi/janus-machine-market-search-github-ingress-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/janus-machine-market/refs/heads/main/authentication/janus-machine-market-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- Research
- Search
- Provenance
- Code Review
- GitHub Issues
- Agent Marketplace
---
