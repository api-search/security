---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nahook-com-openapi-generated.yml
  format: yaml
  label: Nahook API
  slug: nahook-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nahook-com/openapi/_ae-authored/nahook-com-openapi-generated.yml
auth_types: []
description: Authentication methods for Nahook APIs
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Nahook Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nahook declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Nahook
provider_slug: nahook-com
scheme_count: 3
schemes:
- evidence: 'Header: Authorization: Bearer nhk_...'
  header: Authorization
  how_to_obtain: Create them in the dashboard under API Keys, selecting the target environment. The full key is only shown once at creation.
  location: header
  name: API Key
  type: http-bearer
- evidence: 'Header: Authorization: Bearer nhm_...'
  header: Authorization
  how_to_obtain: Created in the dashboard under Management Tokens; you can set expiration (30 days, 90 days, 1 year, or never).
  location: header
  name: Management Token
  type: http-bearer
- evidence: Portal sessions authenticate requests from the Developer Portal — the embeddable UI where your customers manage their own endpoints.
  header: Authorization
  how_to_obtain: Short-lived sessions are created via the Management API (see Embedding the Portal for the full flow).
  location: header
  name: Portal Session
  type: http-bearer
slug: nahook-com-authentication
source_filename: nahook-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.nahook.com/authentication/
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.nahook.com/authentication/\nsources:\n- https://docs.nahook.com/authentication/\n- https://docs.nahook.com/authentication/\n- https://docs.nahook.com/quickstart/\n- https://docs.nahook.com/quickstart/\ndescription: Authentication methods for Nahook APIs\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Header: Authorization: Bearer nhk_...'\n  location: header\n  header: Authorization\n  how_to_obtain: Create them in the dashboard under API Keys, selecting the target environment. The full key is only shown once at creation.\n- type: http-bearer\n  name: Management Token\n  evidence: 'Header: Authorization: Bearer nhm_...'\n  location: header\n  header: Authorization\n  how_to_obtain: Created in the dashboard under Management Tokens; you can set expiration (30 days, 90 days, 1 year, or never).\n- type: http-bearer\n  name: Portal Session\n  evidence: Portal\
  \ sessions authenticate requests from the Developer Portal — the embeddable UI where your customers manage their own endpoints.\n  location: header\n  header: Authorization\n  how_to_obtain: Short-lived sessions are created via the Management API (see Embedding the Portal for the full flow).\ndocs: https://docs.nahook.com/authentication/\n"
source_yaml_url: https://artifacts.apis.io/nahook-com/authentication/nahook-com-authentication.yml
summary_line: 3 schemes
tags:
- Webhook
- Software-as-a-Service
- Developer Tools
- Automation
---
