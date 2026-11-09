---
anonymous_access: false
api_key_in: []
api_specs:
- filename: usagerail-openapi-generated.yml
  format: yaml
  label: UsageRail API
  slug: usagerail-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usagerail/openapi/_ae-authored/usagerail-openapi-generated.yml
auth_types: []
description: UsageRail authenticates clients using API keys.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Usagerail Authentication
name_suffix: Authentication
oauth_flows: []
overview: UsageRail declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: UsageRail
provider_slug: usagerail
scheme_count: 2
schemes:
- evidence: 'The key comes from the Authorization: Bearer header, or from x-api-key when the request has no bearer token.'
  header: Authorization
  location: header
  name: api-key
  type: apiKey
- evidence: 'The key comes from the Authorization: Bearer header, or from x-api-key when the request has no bearer token.'
  header: x-api-key
  location: header
  name: api-key
  type: apiKey
slug: usagerail-authentication
source_filename: usagerail-authentication.yml
source_heading: Authentication Profile
source_url: https://usagerail.com/docs/express
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://usagerail.com/docs/express\nsources:\n- https://usagerail.com/docs/express\n- https://usagerail.com/docs/hono\n- https://usagerail.com/docs/fastify\n- https://usagerail.com/docs/nextjs\ndescription: UsageRail authenticates clients using API keys.\nschemes:\n- type: apiKey\n  name: api-key\n  evidence: 'The key comes from the Authorization: Bearer header, or from x-api-key when the request has no bearer token.'\n  location: header\n  header: Authorization\n- type: apiKey\n  name: api-key\n  evidence: 'The key comes from the Authorization: Bearer header, or from x-api-key when the request has no bearer token.'\n  location: header\n  header: x-api-key\ndocs: https://usagerail.com/docs/express\n"
source_yaml_url: https://artifacts.apis.io/usagerail/authentication/usagerail-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API Monetization
- Software-as-a-Service
- Billing
- Rate Limiting
- Developer Tools
---
