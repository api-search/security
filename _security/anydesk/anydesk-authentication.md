---
api_key_in:
- header
auth_types:
- apiKey
description: The AnyDesk my.anydesk I REST API authenticates with a License ID and an API Password supplied in an authentication request header. Credentials are issued by AnyDesk support against a customer number (On-Premises licenses generate them via the console REST-API command). No OpenAPI is published, so this profile is captured from the documentation rather than derived from a spec.
kind: authentication
layout: security
method: searched
name: Anydesk Authentication
name_suffix: Authentication
oauth_flows: []
overview: AnyDesk secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AnyDesk
provider_slug: anydesk
scheme_count: 1
schemes:
- description: Requests are authenticated with the account License ID plus an API Password, passed in the request authentication header documented in the Files tab of the my.anydesk.com customer portal. Credentials are requested from AnyDesk support with a customer number.
  in: header
  name: LicenseCredentials
  sources:
  - https://support.anydesk.com/docs/rest-api
  type: apiKey
slug: anydesk-authentication
source_filename: anydesk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: searched\nsource: https://support.anydesk.com/docs/rest-api\ndocs: https://support.anydesk.com/docs/rest-api\ndescription: >-\n  The AnyDesk my.anydesk I REST API authenticates with a License ID and an API\n  Password supplied in an authentication request header. Credentials are issued\n  by AnyDesk support against a customer number (On-Premises licenses generate\n  them via the console REST-API command). No OpenAPI is published, so this\n  profile is captured from the documentation rather than derived from a spec.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n  - name: LicenseCredentials\n    type: apiKey\n    in: header\n    description: >-\n      Requests are authenticated with the account License ID plus an API\n      Password, passed in the request authentication header documented in the\n      Files tab of the my.anydesk.com customer portal. Credentials are requested\n      from AnyDesk support\
  \ with a customer number.\n    sources:\n    - https://support.anydesk.com/docs/rest-api\nnotes: >-\n  The exact header name and endpoint domain are published inside the customer\n  portal (my.anydesk.com Files tab) and the On-Premises Installation Guide, not\n  on the public web. This artifact records the documented auth model without\n  reproducing gated credential material.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anydesk/refs/heads/main/authentication/anydesk-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Remote Work
- Remote Desktop
- Remote Access
- Remote Support
- IT Management
- REST API
- Security
---
