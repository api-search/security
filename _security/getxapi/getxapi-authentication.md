---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication schemes for GetXAPI
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Getxapi Authentication
name_suffix: Authentication
oauth_flows: []
overview: GetXAPI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GetXAPI
provider_slug: getxapi
scheme_count: 1
schemes:
- evidence: All requests require an API key passed as a Bearer token in the Authorization header.
  header: Authorization
  location: header
  name: Bearer
  type: http-bearer
slug: getxapi-authentication
source_filename: getxapi-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.getxapi.com/docs
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.getxapi.com/docs\nsources:\n- https://docs.getxapi.com/docs\ndescription: Authentication schemes for GetXAPI\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: All requests require an API key passed as a Bearer token in the Authorization header.\n  location: header\n  header: Authorization\ndocs: https://docs.getxapi.com/docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/getxapi/refs/heads/main/authentication/getxapi-authentication.yml
summary_line: 1 scheme
tags:
- Company
- API
- Twitter
- Tools
- Documentation
---
