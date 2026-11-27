---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentbill-dev-openapi-generated.yml
  format: yaml
  label: AgentBill API
  slug: agentbill-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentbill-dev/openapi/_ae-authored/agentbill-dev-openapi-generated.yml
auth_types: []
description: AgentBill uses an API key that is sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: AgentBill Authentication
name_suffix: Authentication
oauth_flows: []
overview: AgentBill declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AgentBill
provider_slug: agentbill-dev
scheme_count: 1
schemes:
- evidence: 'The Node SDK exports functions rather than a client object and reads AGENTBILL_API_KEY itself, so on a host with no shell you set the variable in the platform''s own config, or skip the SDK and send an Authorization: Bearer header yourself.'
  header: Authorization
  how_to_obtain: Get API key from the console (shown once after sign‑up).
  location: header
  name: Authorization
  type: apiKey
slug: agentbill-dev-authentication
source_filename: agentbill-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://agentbill.dev/register
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agentbill.dev/register\nsources:\n- https://agentbill.dev/register\n- https://agentbill.dev/docs/first-run\ndescription: AgentBill uses an API key that is sent as a Bearer token in the Authorization header.\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'The Node SDK exports functions rather than a client object and reads AGENTBILL_API_KEY itself, so on a host with no shell you set\n    the variable in the platform''s own config, or skip the SDK and send an Authorization: Bearer header yourself.'\n  location: header\n  header: Authorization\n  how_to_obtain: Get API key from the console (shown once after sign‑up).\nnote: No OAuth2, HTTP Basic, JWT, HMAC, MTLS, or other authentication schemes are documented on the provided pages.\ndocs: https://agentbill.dev/register\n"
source_yaml_url: https://artifacts.apis.io/agentbill-dev/authentication/agentbill-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
---
