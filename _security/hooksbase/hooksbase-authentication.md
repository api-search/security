---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hooksbase-openapi-generated.yml
  format: yaml
  label: Hooksbase API
  slug: hooksbase-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hooksbase/refs/heads/main/openapi/_ae-authored/hooksbase-openapi-generated.yml
auth_types: []
description: 'Hooksbase provides three authentication models: session auth for the dashboard, project API keys for the Public API, and webhook ingest secrets for sending events to a webhook’s ingest URL.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Hooksbase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hooksbase declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Hooksbase
provider_slug: hooksbase
scheme_count: 3
schemes:
- evidence: The Hooksbase dashboard uses your browser session. It is a product UI, not part of the Public API, and is not reachable with a project API key.
  how_to_obtain: Obtained automatically via browser login to the Hooksbase dashboard.
  name: Dashboard session auth
  type: other
- evidence: 'The Public API uses Authorization: Bearer swk_... . Use this for webhook configuration, delivery history, replay, usage, and other automation-friendly routes.'
  header: Authorization
  how_to_obtain: Create a project API key in the dashboard under project settings or via the Public API.
  location: header
  name: Project API key
  type: http-bearer
- evidence: The public ingest surface uses the webhook's whsec_... secret against the webhook-specific ingest URL.
  header: Authorization
  how_to_obtain: Returned once on webhook creation or when rotating the ingest secret.
  location: header
  name: Public ingest secret
  type: http-bearer
slug: hooksbase-authentication
source_filename: hooksbase-authentication.yml
source_heading: Authentication Profile
source_url: https://www.hooksbase.com/docs/authentication
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.hooksbase.com/docs/authentication\nsources:\n- https://www.hooksbase.com/docs/authentication\n- https://www.hooksbase.com/guides/receive-stripe-webhooks\n- https://www.hooksbase.com/docs/quickstart\n- https://www.hooksbase.com/docs/onboarding\ndescription: 'Hooksbase provides three authentication models: session auth for the dashboard, project API keys for the Public API, and webhook\n  ingest secrets for sending events to a webhook’s ingest URL.'\nschemes:\n- type: other\n  name: Dashboard session auth\n  evidence: The Hooksbase dashboard uses your browser session. It is a product UI, not part of the Public API, and is not reachable with a project\n    API key.\n  how_to_obtain: Obtained automatically via browser login to the Hooksbase dashboard.\n- type: http-bearer\n  name: Project API key\n  evidence: 'The Public API uses Authorization: Bearer swk_... . Use this\
  \ for webhook configuration, delivery history, replay, usage, and other\n    automation-friendly routes.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a project API key in the dashboard under project settings or via the Public API.\n- type: http-bearer\n  name: Public ingest secret\n  evidence: The public ingest surface uses the webhook's whsec_... secret against the webhook-specific ingest URL.\n  location: header\n  header: Authorization\n  how_to_obtain: Returned once on webhook creation or when rotating the ingest secret.\ndocs: https://www.hooksbase.com/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hooksbase/refs/heads/main/authentication/hooksbase-authentication.yml
summary_line: 3 schemes
tags:
- Company
- EventInfrastructure
- AI
- Webhooks
- Automation
- Integration
---
