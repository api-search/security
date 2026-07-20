---
api_key_in:
- basic-auth
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Illumio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Illumio secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Illumio
provider_slug: illumio
scheme_count: 1
schemes:
- description: 'The Illumio PCE REST API authenticates with an organization-scoped API key presented via HTTP Basic authentication: the API key ID (or a username) is the Basic-auth username and the API key secret (or password) is the Basic-auth password. API keys are created per user in the PCE and are scoped to an organization (org_id). Session tokens are also available for short-lived, browser-derived access.'
  name: apiKeyBasic
  scheme: basic
  sources:
  - docs
  type: http
slug: illumio-authentication
source_filename: illumio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://product-docs-repo.illumio.com/Tech-Docs/Core/24.4/REST-APIs/out/en/index-en.html\ndocs: https://docs.illumio.com/core/\nsummary:\n  types: [http]\n  http_scheme: basic\n  api_key_in: [basic-auth]\n  oauth2_flows: []\nschemes:\n- name: apiKeyBasic\n  type: http\n  scheme: basic\n  description: >-\n    The Illumio PCE REST API authenticates with an organization-scoped API key\n    presented via HTTP Basic authentication: the API key ID (or a username) is\n    the Basic-auth username and the API key secret (or password) is the\n    Basic-auth password. API keys are created per user in the PCE and are scoped\n    to an organization (org_id). Session tokens are also available for\n    short-lived, browser-derived access.\n  sources: [docs]\nnotes:\n- API requests are made against the customer/tenant PCE FQDN at the /api/v2 base path over HTTPS.\n- Requests are org-scoped; most collection/instance URIs embed /orgs/{org_id}/.\n\
  - The official illumio Python client sets credentials via pce.set_credentials(api_key, api_secret).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/illumio/refs/heads/main/authentication/illumio-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Security
- Cybersecurity
- Zero Trust
- Microsegmentation
- Cloud Security
- Networking
- Workload Protection
- Ransomware
- Endpoint Security
---
