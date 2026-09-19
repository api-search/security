---
anonymous_access: false
api_key_in: []
api_specs:
- filename: augmentt-customers-api-openapi.yml
  format: yaml
  label: Augmentt Customers API
  slug: augmentt-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augmentt/refs/heads/main/openapi/augmentt-customers-api-openapi.yml
- filename: augmentt-licensing-api-openapi.yml
  format: yaml
  label: Augmentt Licensing API
  slug: augmentt-licensing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augmentt/refs/heads/main/openapi/augmentt-licensing-api-openapi.yml
- filename: augmentt-security-reports-api-openapi.yml
  format: yaml
  label: Augmentt Security Reports API
  slug: augmentt-security-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/augmentt/refs/heads/main/openapi/augmentt-security-reports-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Augmentt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Augmentt declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Augmentt
provider_slug: augmentt
scheme_count: 0
schemes: []
slug: augmentt-authentication
source_filename: augmentt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://support.augmentt.com/kb/en/augmentt-api-548051\nprovider: Augmentt\nproviderId: augmentt\ndocs: https://support.augmentt.com/kb/en/augmentt-api-548051\nsummary: >-\n  The Augmentt API authenticates with a paired API key: two custom headers, AccessKeyId and\n  AccessKeySecret, sent together on every request. There is no OAuth, no OpenID Connect, no bearer\n  token and no mTLS. Keys are issued by Augmentt support on request — they cannot be generated or\n  rotated self-service in the portal — and the secret cannot be retrieved again after issue.\napis:\n  - name: Augmentt API\n    spec: openapi/augmentt-api-openapi.yml\n    hosts:\n      - https://api.augmentt.com\n      - https://api.eu.augmentt.com\n      - https://api.apac.augmentt.com\n    schemes:\n      - id: AccessKeyId\n        type: apiKey\n        in: header\n        name: AccessKeyId\n        required: true\n        description: Access Key ID provided by the\
  \ Augmentt team.\n      - id: AccessKeySecret\n        type: apiKey\n        in: header\n        name: AccessKeySecret\n        required: true\n        description: >-\n          Access Key Secret provided by the Augmentt team. Treat it like a password; it cannot be\n          retrieved from the portal after issue.\n    applied: all-operations\n    combination: both-headers-required\n    oauth2: false\n    openid_connect: false\n    mutual_tls: false\n    bearer: false\ncredential_lifecycle:\n  issuance: manual\n  issued_by: Augmentt support (support@augmentt.com)\n  self_service: false\n  request_requires: [Augmentt organization name, description of the intended integration]\n  rotation: >-\n    Contact support for a new key pair. There is no documented self-service rotation or expiry, and\n    no published key-listing or revocation endpoint.\n  retrievable_after_issue: false\n  scopes: none\n  eligibility: >-\n    API access is enabled per organization and is available to partners on\
  \ Autopilot. Valid keys\n    against an organization without API access enabled return HTTP 403 FORBIDDEN.\n  trial_access: >-\n    Available during a trial; the Augmentt account manager makes the key request on the customer's\n    behalf.\nfailure_modes:\n  - status: 401\n    error: UNAUTHORIZED\n    cause: >-\n      Missing or invalid credentials. The docs call out header name spelling (exactly AccessKeyId and\n      AccessKeySecret) and stray whitespace in the values as the common causes.\n  - status: 403\n    error: FORBIDDEN\n    cause: Keys are valid, but API access is not enabled for the organization.\nnotes:\n  - Read-only API — every endpoint is GET and no request body is accepted.\n  - >-\n    The same key pair is scoped to one Augmentt organization; a customerId from a different\n    organization returns 404 NOT_FOUND.\n  - >-\n    Regional isolation: NAM, EU and APAC are separate hosts. The documentation does not state whether\n    a key issued in one region is valid in another.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/augmentt/refs/heads/main/authentication/augmentt-authentication.yml
summary_line: 0 schemes
tags:
- MSP
- Microsoft-365
- SaaS Management
- SaaS Security
- Shadow IT
- Security Posture
- Compliance
- License Management
- Multi-Tenant
- Reporting
---
