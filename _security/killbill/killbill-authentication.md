---
anonymous_access: false
api_key_in: []
api_specs:
- filename: killbill-api-openapi.json
  format: json
  label: Kill Bill Api API
  slug: kill-bill-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/killbill/openapi/_original/killbill-api-openapi.json
auth_types: []
description: Authentication for Kill Bill API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Kill Bill Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kill Bill declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Kill Bill
provider_slug: killbill
scheme_count: 3
schemes:
- evidence: 'curl -v \ -X POST \ -u admin:password \ -H ''X-Killbill-ApiKey: bob'' \ -H ''X-Killbill-ApiSecret: lazar'' ...'
  name: Basic Auth
  type: http-basic
- evidence: '-H ''X-Killbill-ApiKey: bob'''
  header: X-Killbill-ApiKey
  location: header
  name: X-Killbill-ApiKey
  type: apiKey
- evidence: '-H ''X-Killbill-ApiSecret: lazar'''
  header: X-Killbill-ApiSecret
  location: header
  name: X-Killbill-ApiSecret
  type: apiKey
slug: killbill-authentication
source_filename: killbill-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.killbill.io/latest/getting_started
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.killbill.io/latest/getting_started\nsources:\n- https://docs.killbill.io/latest/getting_started\n- https://docs.killbill.io/latest/quick_start_with_kaui\n- https://docs.killbill.io/latest/quick_start_with_kb_api\n- https://docs.killbill.io/latest/PostgreSQL\ndescription: Authentication for Kill Bill API\nschemes:\n- type: http-basic\n  name: Basic Auth\n  evidence: 'curl -v \\ -X POST \\ -u admin:password \\ -H ''X-Killbill-ApiKey: bob'' \\ -H ''X-Killbill-ApiSecret: lazar'' ...'\n- type: apiKey\n  name: X-Killbill-ApiKey\n  evidence: '-H ''X-Killbill-ApiKey: bob'''\n  location: header\n  header: X-Killbill-ApiKey\n- type: apiKey\n  name: X-Killbill-ApiSecret\n  evidence: '-H ''X-Killbill-ApiSecret: lazar'''\n  location: header\n  header: X-Killbill-ApiSecret\nnote: No OAuth2 flows are documented on the provided pages.\ndocs: https://docs.killbill.io/latest/getting_started\n"
source_yaml_url: https://artifacts.apis.io/killbill/authentication/killbill-authentication.yml
summary_line: 3 schemes
tags:
- Billing
- Payments
- Subscription Billing
- Usage Metering
- Open Source
- Enterprise Revenue Platform
- Fintech
---
