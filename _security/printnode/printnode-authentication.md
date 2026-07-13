---
api_key_in: []
api_specs:
- filename: printnode-openapi.yml
  format: yaml
  label: PrintNode Computers API
  slug: computers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-openapi.yml
- filename: printnode-openapi.yml
  format: yaml
  label: PrintNode Printers API
  slug: printers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-openapi.yml
- filename: printnode-openapi.yml
  format: yaml
  label: PrintNode PrintJobs API
  slug: printjobs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-openapi.yml
- filename: printnode-openapi.yml
  format: yaml
  label: PrintNode Scales API
  slug: scales
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-openapi.yml
- filename: printnode-openapi.yml
  format: yaml
  label: PrintNode Account and API Keys API
  slug: account-api-keys
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-openapi.yml
- filename: printnode-openapi.yml
  format: yaml
  label: PrintNode Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Printnode Authentication
name_suffix: Authentication
oauth_flows: []
overview: PrintNode secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PrintNode
provider_slug: printnode
scheme_count: 1
schemes:
- description: HTTP Basic authentication. Supply the PrintNode API key as the username and leave the password empty. Integrator accounts may additionally authenticate on behalf of a child account using the X-Child-Account-By-Id, X-Child-Account-By-Email, or X-Child-Account-By-CreatorRef header.
  name: apiKeyBasicAuth
  scheme: basic
  sources:
  - openapi/printnode-openapi.yml
  type: http
slug: printnode-authentication
source_filename: printnode-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/printnode-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKeyBasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Supply the PrintNode API key as the username and leave\n    the password empty. Integrator accounts may additionally authenticate on behalf of a child\n    account using the X-Child-Account-By-Id, X-Child-Account-By-Email, or X-Child-Account-By-CreatorRef\n    header.\n  sources:\n  - openapi/printnode-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/authentication/printnode-authentication.yml
summary_line: http · 1 scheme
tags:
- Printing
- Cloud Printing
- Remote Printing
- Print Jobs
- Hardware
---
