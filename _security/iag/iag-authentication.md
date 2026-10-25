---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: none
name: Iag Authentication
name_suffix: Authentication
oauth_flows: []
overview: Insurance Australia Group declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Insurance Australia Group
provider_slug: iag
scheme_count: 0
schemes: []
slug: iag-authentication
source_filename: iag-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Insurance Australia Group authentication\ngenerated: '2026-10-20'\nmethod: none\nsource:\n- https://api.iag.com.au/\n- https://docs.iag.com.au/\nnote: >-\n  Checked, nothing to record. IAG publishes no OpenAPI contract and no API\n  authentication documentation. On 2026-10-20 https://api.iag.com.au/,\n  https://api.cgu.com.au/, https://api.nrma.com.au/ and\n  https://test-api.iag.com.au/ each returned HTTP 404 with an Apigee\n  ApplicationNotFound fault (\"Unable to identify proxy for host\") and no\n  WWW-Authenticate challenge, so no API auth scheme is observable.\n  https://docs.iag.com.au/ returned HTTP 401 with\n  'www-authenticate: Bearer realm=\"docs.iag.com.au\"' and an authorization_uri on\n  login.microsoftonline.com (Microsoft Entra ID): that is a workforce sign-in\n  wall in front of an internal docs site, not a documented API scheme, so it is\n  not recorded as one.\nschemes: []\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iag/refs/heads/main/authentication/iag-authentication.yml
summary_line: 0 schemes
tags:
- Insurance
- Australia
- New Zealand
- Property and Casualty
- General Insurance
- Carrier
- Underwriting
- Claims
---
