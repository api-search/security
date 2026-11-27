---
anonymous_access: false
api_key_in: []
api_specs:
- filename: impri-dev-actions-api-openapi.yml
  format: yaml
  label: Impri Actions API
  slug: impri-dev-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-actions-api-openapi.yml
- filename: impri-dev-billing-api-openapi.yml
  format: yaml
  label: Impri Billing API
  slug: impri-dev-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-billing-api-openapi.yml
- filename: impri-dev-keys-api-openapi.yml
  format: yaml
  label: Impri Keys API
  slug: impri-dev-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-keys-api-openapi.yml
- filename: impri-dev-notification-channels-api-openapi.yml
  format: yaml
  label: Impri Notification Channels API
  slug: impri-dev-notification-channels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-notification-channels-api-openapi.yml
- filename: impri-dev-project-api-openapi.yml
  format: yaml
  label: Impri Project API
  slug: impri-dev-project-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-project-api-openapi.yml
- filename: impri-dev-push-api-openapi.yml
  format: yaml
  label: Impri Push API
  slug: impri-dev-push-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-push-api-openapi.yml
- filename: impri-dev-watchers-api-openapi.yml
  format: yaml
  label: Impri Watchers API
  slug: impri-dev-watchers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/impri-dev/openapi/impri-dev-watchers-api-openapi.yml
auth_types: []
description: Authentication for Impri API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Impri Authentication
name_suffix: Authentication
oauth_flows: []
overview: Impri declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Impri
provider_slug: impri-dev
scheme_count: 1
schemes:
- evidence: Every request to the Impri API is authenticated with a Bearer token that looks like im_<base64url> .
  header: Authorization
  how_to_obtain: Create an API key via the Impri API (POST /v1/keys) or the web UI; the raw key is shown once and must be stored securely. The key value is then used as a Bearer token in the Authorization header.
  location: header
  name: Bearer token
  type: http-bearer
slug: impri-dev-authentication
source_filename: impri-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://impri.dev/docs/api-keys
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://impri.dev/docs/api-keys\nsources:\n- https://impri.dev/docs/api-keys\n- https://impri.dev/docs/quickstart\ndescription: Authentication for Impri API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: Every request to the Impri API is authenticated with a Bearer token that looks like im_<base64url> .\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key via the Impri API (POST /v1/keys) or the web UI; the raw key is shown once and must be stored securely. The\n    key value is then used as a Bearer token in the Authorization header.\ndocs: https://impri.dev/docs/api-keys\n"
source_yaml_url: https://artifacts.apis.io/impri-dev/authentication/impri-dev-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Human-in-the-Loop
- Approval
- Automation
- Software-as-a-Service
---
