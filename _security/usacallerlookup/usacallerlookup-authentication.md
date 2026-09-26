---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: derived
name: Usacallerlookup Authentication
name_suffix: Authentication
oauth_flows: []
overview: USACallerLookup declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: USACallerLookup
provider_slug: usacallerlookup
scheme_count: 0
schemes: []
slug: usacallerlookup-authentication
source_filename: usacallerlookup-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: derived\nsource: openapi/usacallerlookup-openapi.json\nsummary: >-\n  Public, unauthenticated API. The OpenAPI 3.1.0 contract declares no securitySchemes and\n  no security requirement on any operation. No API key, token, or sign-up is required; the\n  only access control is a 60-request-per-minute-per-IP rate limit.\nschemes: []\npublic: true\nsignup_required: false\nnotes:\n  - All three operations (lookupNumber, getAreaCode, getStats) are anonymous HTTP GET.\n  - Abuse control is per-IP rate limiting, not credentials (see rate-limits/).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usacallerlookup/refs/heads/main/authentication/usacallerlookup-authentication.yml
summary_line: 0 schemes
tags:
- Phone Lookup
- Caller ID
- robocall
- FTC
- Telecommunications
- Open Data
- Fraud Prevention
---
