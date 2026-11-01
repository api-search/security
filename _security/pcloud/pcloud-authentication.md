---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Pcloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: pCloud declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: pCloud
provider_slug: pcloud
scheme_count: 1
schemes:
- description: Authentication token passed as 'auth' query parameter.
  in: query
  name: auth
  type: apiKey
slug: pcloud-authentication
source_filename: pcloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://docs.pcloud.com/methods/intro/authentication.html\nschemes:\n  - type: apiKey\n    name: auth\n    in: query\n    description: Authentication token passed as 'auth' query parameter.\n"
source_yaml_url: https://artifacts.apis.io/pcloud/authentication/pcloud-authentication.yml
summary_line: 1 scheme
tags:
- Cloud Storage
- File Sync
- Backup
- Security
- Collaboration
---
