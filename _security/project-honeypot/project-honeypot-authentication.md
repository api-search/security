---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Project Honeypot Authentication
name_suffix: Authentication
oauth_flows: []
overview: Project Honey Pot declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Project Honey Pot
provider_slug: project-honeypot
scheme_count: 1
schemes:
- description: Access Key is a 12-character lower-case string included as the first label in the DNS query for http:BL.
  in: dns
  name: Access Key
  type: apiKey
slug: project-honeypot-authentication
source_filename: project-honeypot-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource: https://projecthoneypot.org/httpbl_api.php\nschemes:\n  - type: apiKey\n    name: Access Key\n    in: dns\n    description: \"Access Key is a 12-character lower-case string included as the first label in the DNS query for http:BL.\"\n"
source_yaml_url: https://artifacts.apis.io/project-honeypot/authentication/project-honeypot-authentication.yml
summary_line: 1 scheme
tags:
- Anti‑Spam
- Security
- Community
- Fraud Prevention
- Open Data
---
