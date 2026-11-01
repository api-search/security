---
anonymous_access: false
api_key_in: []
api_specs:
- filename: uptime-kuma-openapi-generated.yml
  format: yaml
  label: Uptime Kuma API
  slug: uptime-kuma-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uptime-kuma/openapi/_ae-authored/uptime-kuma-openapi-generated.yml
auth_types: []
description: Authentication schemes for Uptime Kuma Prometheus metrics endpoint
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Uptime Kuma Authentication
name_suffix: Authentication
oauth_flows: []
overview: Uptime Kuma declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Uptime Kuma
provider_slug: uptime-kuma
scheme_count: 1
schemes:
- evidence: Authentication is done by passing the API key in the Authorization header.
  header: Authorization
  how_to_obtain: Generate an API key on the API Keys page in settings; the key is shown once in a pop‑up dialog.
  location: header
  name: API Key
  type: http-basic
slug: uptime-kuma-authentication
source_filename: uptime-kuma-authentication.yml
source_heading: Authentication Profile
source_url: https://uptime.kuma.pet/docs/Prometheus-API-Keys
source_yaml: "generated: '2026-10-28'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://uptime.kuma.pet/docs/Prometheus-API-Keys\nsources:\n- https://uptime.kuma.pet/docs/Prometheus-API-Keys\n- https://uptime.kuma.pet/docs/Setup-Development-Environment\ndescription: Authentication schemes for Uptime Kuma Prometheus metrics endpoint\nschemes:\n- type: http-basic\n  name: API Key\n  evidence: Authentication is done by passing the API key in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an API key on the API Keys page in settings; the key is shown once in a pop‑up dialog.\ndocs: https://uptime.kuma.pet/docs/Prometheus-API-Keys\n"
source_yaml_url: https://artifacts.apis.io/uptime-kuma/authentication/uptime-kuma-authentication.yml
summary_line: 1 scheme
tags:
- Monitoring
- Self-Hosted
- Open-Source
- Dashboard
- Alerts
---
