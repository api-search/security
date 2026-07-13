---
api_key_in: []
api_specs:
- filename: rocket-lawyer-authentication-api-openapi.yml
  format: yaml
  label: Rocket Lawyer Authentication API
  slug: rocket-lawyer-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-lawyer/refs/heads/main/openapi/rocket-lawyer-authentication-api-openapi.yml
- filename: rocket-lawyer-rocketdocument-api-openapi.yml
  format: yaml
  label: Rocket Lawyer RocketDocument v2 API
  slug: rocket-lawyer-rocketdocument-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-lawyer/refs/heads/main/openapi/rocket-lawyer-rocketdocument-api-openapi.yml
- filename: rocket-lawyer-rocketsign-binders-api-openapi.yml
  format: yaml
  label: Rocket Lawyer RocketSign and Binders API
  slug: rocket-lawyer-rocketsign-binders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-lawyer/refs/heads/main/openapi/rocket-lawyer-rocketsign-binders-api-openapi.yml
- filename: rocket-lawyer-events-api-openapi.yml
  format: yaml
  label: Rocket Lawyer Events API
  slug: rocket-lawyer-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocket-lawyer/refs/heads/main/openapi/rocket-lawyer-events-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rocket Lawyer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rocket Lawyer secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Rocket Lawyer
provider_slug: rocket-lawyer
scheme_count: 1
schemes:
- name: BearerTokenAuth
  scheme: bearer
  sources:
  - openapi/rocket-lawyer-authentication-api-openapi.yml
  - openapi/rocket-lawyer-events-api-openapi.yml
  - openapi/rocket-lawyer-rocketdocument-api-openapi.yml
  - openapi/rocket-lawyer-rocketsign-binders-api-openapi.yml
  type: http
slug: rocket-lawyer-authentication
source_filename: rocket-lawyer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/rocket-lawyer-authentication-api-openapi.yml, openapi/rocket-lawyer-events-api-openapi.yml,\n  openapi/rocket-lawyer-rocketdocument-api-openapi.yml, openapi/rocket-lawyer-rocketsign-binders-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerTokenAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/rocket-lawyer-authentication-api-openapi.yml\n  - openapi/rocket-lawyer-events-api-openapi.yml\n  - openapi/rocket-lawyer-rocketdocument-api-openapi.yml\n  - openapi/rocket-lawyer-rocketsign-binders-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocket-lawyer/refs/heads/main/authentication/rocket-lawyer-authentication.yml
summary_line: http · 1 scheme
tags:
- Legal
- Legal Technology
- LegalTech
- Legal Documents
- Electronic Signature
- eSignature
- Document Creation
- Document Management
- Business Formation
- LLC Formation
- Registered Agent
- Trademark
- Wills
- Estate Planning
- Attorney Network
- Small Business
- Membership
- Embedded UX
- Partner API
- Apigee
- OpenAPI
---
