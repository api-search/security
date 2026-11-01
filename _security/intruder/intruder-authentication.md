---
anonymous_access: false
api_key_in: []
api_specs:
- filename: intruder-health-api-openapi.yml
  format: yaml
  label: Intruder Health API
  slug: intruder-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-health-api-openapi.yml
- filename: intruder-issues-api-openapi.yml
  format: yaml
  label: Intruder Issues API
  slug: intruder-issues-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-issues-api-openapi.yml
- filename: intruder-licenses-api-openapi.yml
  format: yaml
  label: Intruder Licenses API
  slug: intruder-licenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-licenses-api-openapi.yml
- filename: intruder-occurrences-api-openapi.yml
  format: yaml
  label: Intruder Occurrences API
  slug: intruder-occurrences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-occurrences-api-openapi.yml
- filename: intruder-scans-api-openapi.yml
  format: yaml
  label: Intruder Scans API
  slug: intruder-scans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-scans-api-openapi.yml
- filename: intruder-tags-api-openapi.yml
  format: yaml
  label: Intruder Tags API
  slug: intruder-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-tags-api-openapi.yml
- filename: intruder-targets-api-openapi.yml
  format: yaml
  label: Intruder Targets API
  slug: intruder-targets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intruder/openapi/intruder-targets-api-openapi.yml
auth_types: []
description: Authentication schemes for Intruder target authentications
kind: authentication
layout: security
mechanism_count: 7
method: searched
name: Intruder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Intruder declares 7 security scheme(s) across its OpenAPI definitions.
provider_name: Intruder
provider_slug: intruder
scheme_count: 7
schemes:
- evidence: http_header - HTTP_HEADER
  name: HTTP_HEADER
  type: http_header
- evidence: session_cookie - SESSION_COOKIE
  name: SESSION_COOKIE
  type: session_cookie
- evidence: http - HTTP
  name: HTTP
  type: http
- evidence: form - FORM
  name: FORM
  type: form
- evidence: recorded - RECORDED
  name: RECORDED
  type: recorded
- evidence: unauthenticated - UNAUTHENTICATED
  name: UNAUTHENTICATED
  type: unauthenticated
- evidence: oauth_client_credentials - OAUTH_CLIENT_CREDENTIALS
  name: OAUTH_CLIENT_CREDENTIALS
  type: oauth_client_credentials
slug: intruder-authentication
source_filename: intruder-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.intruder.io/reference/targets_authentications_create.md
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.intruder.io/reference/targets_authentications_create.md\nsources:\n- https://developers.intruder.io/reference/targets_authentications_create.md\n- https://developers.intruder.io/reference/targets_authentications_partial_update.md\n- https://developers.intruder.io/reference/targets_authentications_destroy.md\n- https://developers.intruder.io/reference/targets_authentications_create\ndescription: Authentication schemes for Intruder target authentications\nschemes:\n- type: http_header\n  name: HTTP_HEADER\n  evidence: http_header - HTTP_HEADER\n- type: session_cookie\n  name: SESSION_COOKIE\n  evidence: session_cookie - SESSION_COOKIE\n- type: http\n  name: HTTP\n  evidence: http - HTTP\n- type: form\n  name: FORM\n  evidence: form - FORM\n- type: recorded\n  name: RECORDED\n  evidence: recorded - RECORDED\n- type: unauthenticated\n  name: UNAUTHENTICATED\n  evidence:\
  \ unauthenticated - UNAUTHENTICATED\n- type: oauth_client_credentials\n  name: OAUTH_CLIENT_CREDENTIALS\n  evidence: oauth_client_credentials - OAUTH_CLIENT_CREDENTIALS\ndocs: https://developers.intruder.io/reference/targets_authentications_create.md\n"
source_yaml_url: https://artifacts.apis.io/intruder/authentication/intruder-authentication.yml
summary_line: 7 schemes
tags:
- Company
- Security
- Cloud
- API
- AI
- Platform
---
