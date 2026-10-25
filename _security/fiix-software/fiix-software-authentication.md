---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Fiix Software Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fiix Software declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Fiix Software
provider_slug: fiix-software
scheme_count: 1
schemes:
- description: An administrator generates an Application Key, Access Key and Secret Key in the CMMS; the secret cannot be retrieved later. Keys are passed to the Fiix CMMS Client (Java/JavaScript) which signs requests to https://{subdomain}.macmms.com/api.
  name: Fiix API access keys
  type: apiKey
slug: fiix-software-authentication
source_filename: fiix-software-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Fiix Software authentication\ngenerated: '2026-10-20'\nmethod: searched\nsource: https://fiixlabs.github.io/api-documentation/guide.html\ndocs: https://fiixlabs.github.io/api-documentation/guide.html\nschemes:\n- type: apiKey\n  name: Fiix API access keys\n  description: An administrator generates an Application Key, Access Key and Secret Key in the CMMS; the secret cannot be retrieved later. Keys are passed to the Fiix CMMS Client (Java/JavaScript) which signs requests to https://{subdomain}.macmms.com/api.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fiix-software/refs/heads/main/authentication/fiix-software-authentication.yml
summary_line: 1 scheme
tags:
- CMMS
- Maintenance Management
- Asset Management
- Manufacturing
- Reliability
- Work Orders
- SaaS
---
