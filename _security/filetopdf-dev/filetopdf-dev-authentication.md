---
anonymous_access: false
api_key_in: []
api_specs:
- filename: filetopdf-dev-openapi-generated.yml
  format: yaml
  label: FileToPDF.dev API
  slug: filetopdf-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetopdf-dev/openapi/_ae-authored/filetopdf-dev-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: FileToPDF.dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: FileToPDF.dev declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: FileToPDF.dev
provider_slug: filetopdf-dev
scheme_count: 2
schemes:
- description: 'Include your API key in the `x-api-key` header on every request. CORS is

    enabled, so the key can be sent from browser-based clients when that is

    appropriate for your use case.

    '
  in: header
  name: x-api-key
  type: apiKey
- description: 'A Firebase Auth bearer token may be presented via the Authorization

    header (documented via the `invalid_token` / `missing_api_key` error

    codes which reference "Firebase Auth token" explicitly on the

    reference page).

    '
  scheme: bearer
  type: http
slug: filetopdf-dev-authentication
source_filename: filetopdf-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: searched\nsource: https://filetopdf.dev/file\ndocs: https://filetopdf.dev/file\nschemes:\n- type: apiKey\n  name: x-api-key\n  in: header\n  description: |\n    Include your API key in the `x-api-key` header on every request. CORS is\n    enabled, so the key can be sent from browser-based clients when that is\n    appropriate for your use case.\n- type: http\n  scheme: bearer\n  description: |\n    A Firebase Auth bearer token may be presented via the Authorization\n    header (documented via the `invalid_token` / `missing_api_key` error\n    codes which reference \"Firebase Auth token\" explicitly on the\n    reference page).\nerrors:\n- status: 401\n  code: missing_api_key\n  message: No x-api-key header or Authorization token provided.\n- status: 401\n  code: invalid_token\n  message: The provided Firebase Auth token is invalid or expired.\n- status: 403\n  code: forbidden\n  message: Invalid API key, or user is not a member of the workspace.\n\
  notes: |\n  API keys are scoped to a workspace. Paid plans (Basic and above) allow\n  multiple API keys per workspace. Keys are managed in the dashboard.\n"
source_yaml_url: https://artifacts.apis.io/filetopdf-dev/authentication/filetopdf-dev-authentication.yml
summary_line: 2 schemes
tags:
- PDF
- Document Conversion
- HTML to PDF
- Markdown to PDF
- File Conversion
- Headless Chromium
- Developer API
- GDPR
---
