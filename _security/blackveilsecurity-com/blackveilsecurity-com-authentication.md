---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for BlackVeil API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Blackveilsecurity Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BlackVeil declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BlackVeil
provider_slug: blackveilsecurity-com
scheme_count: 1
schemes:
- evidence: Send the key in the Authorization header and keep it out of browser code and source control.
  header: Authorization
  location: header
  name: API key
  type: http-bearer
slug: blackveilsecurity-com-authentication
source_filename: blackveilsecurity-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.blackveilsecurity.com/resources/docs/api
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.blackveilsecurity.com/resources/docs/api\nsources:\n- https://www.blackveilsecurity.com/resources/docs/api\n- https://www.blackveilsecurity.com/resources/docs/quickstart\ndescription: Authentication schemes for BlackVeil API\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: Send the key in the Authorization header and keep it out of browser code and source control.\n  location: header\n  header: Authorization\ndocs: https://www.blackveilsecurity.com/resources/docs/api\n"
source_yaml_url: https://artifacts.apis.io/blackveilsecurity-com/authentication/blackveilsecurity-com-authentication.yml
summary_line: 1 scheme
tags:
- Security
- DNS
- Email Authentication
- Domain Monitoring
- Software-as-a-Service
---
