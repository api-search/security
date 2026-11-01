---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Mozilla Accounts Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mozilla accounts declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Mozilla accounts
provider_slug: mozilla-accounts
scheme_count: 2
schemes:
- description: 'Preferred token scheme using Authorization: Bearer <prefix>_<hex>'
  type: bearer
- description: Legacy fallback token scheme
  type: hawk
slug: mozilla-accounts-authentication
source_filename: mozilla-accounts-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: searched\nsource: https://raw.githubusercontent.com/mozilla/ecosystem-platform/master/docs/reference/authentication-schemes.md\nschemes:\n  - type: bearer\n    description: \"Preferred token scheme using Authorization: Bearer <prefix>_<hex>\"\n  - type: hawk\n    description: \"Legacy fallback token scheme\"\n"
source_yaml_url: https://artifacts.apis.io/mozilla-accounts/authentication/mozilla-accounts-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Authentication
- Identity
- Mozilla
- OpenSource
---
