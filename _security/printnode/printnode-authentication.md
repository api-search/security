---
api_key_in: []
api_specs:
- filename: printnode-account-api-openapi.yml
  format: yaml
  label: PrintNode Account API
  slug: printnode-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-account-api-openapi.yml
- filename: printnode-api-keys-api-openapi.yml
  format: yaml
  label: PrintNode API Keys API
  slug: printnode-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-api-keys-api-openapi.yml
- filename: printnode-clients-api-openapi.yml
  format: yaml
  label: PrintNode Clients API
  slug: printnode-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-clients-api-openapi.yml
- filename: printnode-computers-api-openapi.yml
  format: yaml
  label: PrintNode Computers API
  slug: printnode-computers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-computers-api-openapi.yml
- filename: printnode-printers-api-openapi.yml
  format: yaml
  label: PrintNode Printers API
  slug: printnode-printers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-printers-api-openapi.yml
- filename: printnode-printjobs-api-openapi.yml
  format: yaml
  label: PrintNode PrintJobs API
  slug: printnode-printjobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-printjobs-api-openapi.yml
- filename: printnode-scales-api-openapi.yml
  format: yaml
  label: PrintNode Scales API
  slug: printnode-scales-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-scales-api-openapi.yml
- filename: printnode-utility-api-openapi.yml
  format: yaml
  label: PrintNode Utility API
  slug: printnode-utility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-utility-api-openapi.yml
- filename: printnode-webhooks-api-openapi.yml
  format: yaml
  label: PrintNode Webhooks API
  slug: printnode-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/printnode/refs/heads/main/openapi/printnode-webhooks-api-openapi.yml
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
