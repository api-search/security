---
api_key_in: []
api_specs:
- filename: university-of-zurich-eduid-oidc.yaml
  format: yaml
  label: SWITCH edu-ID / UZH Identity (SAML & OpenID Connect)
  slug: eduid-oidc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-zurich/refs/heads/main/openapi/university-of-zurich-eduid-oidc.yaml
auth_types:
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: derived
name: University Of Zurich Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Zurich secures its APIs with http and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Zurich
provider_slug: university-of-zurich
scheme_count: 2
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/university-of-zurich-eduid-oidc.yaml
  type: http
- name: oidc
  openIdConnectUrl: https://login.eduid.ch/.well-known/openid-configuration
  sources:
  - openapi/university-of-zurich-eduid-oidc.yaml
  type: openIdConnect
slug: university-of-zurich-authentication
source_filename: university-of-zurich-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-zurich-eduid-oidc.yaml\nsummary:\n  types:\n  - http\n  - openIdConnect\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/university-of-zurich-eduid-oidc.yaml\n- name: oidc\n  type: openIdConnect\n  openIdConnectUrl: https://login.eduid.ch/.well-known/openid-configuration\n  sources:\n  - openapi/university-of-zurich-eduid-oidc.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-zurich/refs/heads/main/authentication/university-of-zurich-authentication.yml
summary_line: http/openIdConnect · 2 schemes
tags:
- Education
- Higher Education
- University
- Switzerland
- Open Access
- Research Repository
- Open Data
- Identity
---
