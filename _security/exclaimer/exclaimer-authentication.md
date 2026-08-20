---
api_key_in:
- header
api_specs:
- filename: exclaimer-subscriptions-openapi.yml
  format: yaml
  label: Exclaimer Cloud API
  slug: exclaimer-cloud-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/exclaimer/refs/heads/main/openapi/exclaimer-subscriptions-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Exclaimer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Exclaimer secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Exclaimer
provider_slug: exclaimer
scheme_count: 1
schemes:
- applied: global — declared at the document level, so every one of the 39 operations requires it
  case_note: The prose writes the header as "ExAPIToken" while the securityScheme declares "ExApiToken". HTTP header names are case-insensitive (RFC 9110), so both resolve to the same header.
  failure_mode: '401 Unauthorized when the header is absent or the token is invalid — declared on all 39 operations. Observed live: every path on cloudapi.exclaimer.com returns 401 with an empty body to an anonymous request, except / (the reference page) and /openapi.json (the specification), which are public.'
  in: header
  issuance: Issued by Exclaimer to distributor-network partners out of band. The reference states the header carries "a value that will be provided to you separately". There is no console, no self-service key creation, and no key rotation endpoint in the API.
  name: Exclaimer
  parameter: ExApiToken
  sources:
  - openapi/_original/exclaimer-cloud-api-openapi.json
  - openapi/exclaimer-subscriptions-openapi.yml
  - openapi/exclaimer-msp-openapi.yml
  - openapi/exclaimer-subscription-users-openapi.yml
  - openapi/exclaimer-subscription-transfers-openapi.yml
  - openapi/exclaimer-end-users-openapi.yml
  - openapi/exclaimer-resellers-openapi.yml
  - openapi/exclaimer-mailboxes-openapi.yml
  - openapi/exclaimer-reference-resources-openapi.yml
  - openapi/exclaimer-miscellaneous-openapi.yml
  type: apiKey
slug: exclaimer-authentication
source_filename: exclaimer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  https://cloudapi.exclaimer.com/ (\"Usage\" section of the Exclaimer Cloud API\n  reference), enriched over the derived profile from the securitySchemes in\n  openapi/_original/exclaimer-cloud-api-openapi.json\ndocs: https://cloudapi.exclaimer.com/\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scopes: false\n  self_service_registration: false\nschemes:\n- name: Exclaimer\n  type: apiKey\n  in: header\n  parameter: ExApiToken\n  applied: global — declared at the document level, so every one of the 39 operations requires it\n  issuance: >-\n    Issued by Exclaimer to distributor-network partners out of band. The reference\n    states the header carries \"a value that will be provided to you separately\".\n    There is no console, no self-service key creation, and no key rotation\n    endpoint in the API.\n  failure_mode: >-\n    401 Unauthorized\
  \ when the header is absent or the token is invalid — declared\n    on all 39 operations. Observed live: every path on cloudapi.exclaimer.com\n    returns 401 with an empty body to an anonymous request, except / (the\n    reference page) and /openapi.json (the specification), which are public.\n  case_note: >-\n    The prose writes the header as \"ExAPIToken\" while the securityScheme declares\n    \"ExApiToken\". HTTP header names are case-insensitive (RFC 9110), so both\n    resolve to the same header.\n  sources:\n  - openapi/_original/exclaimer-cloud-api-openapi.json\n  - openapi/exclaimer-subscriptions-openapi.yml\n  - openapi/exclaimer-msp-openapi.yml\n  - openapi/exclaimer-subscription-users-openapi.yml\n  - openapi/exclaimer-subscription-transfers-openapi.yml\n  - openapi/exclaimer-end-users-openapi.yml\n  - openapi/exclaimer-resellers-openapi.yml\n  - openapi/exclaimer-mailboxes-openapi.yml\n  - openapi/exclaimer-reference-resources-openapi.yml\n  - openapi/exclaimer-miscellaneous-openapi.yml\n\
  authorization:\n  model: >-\n    Coarse — permission is a property of the partner account behind the token, not\n    of the token. 403 Forbidden is returned when the token is valid but the caller\n    lacks the required permission, and specifically on the MSP operations when\n    \"the API user is not an MSP type\". There are no scopes and no per-token\n    restriction mechanism.\n  roles_in_api: >-\n    Subscription USERS (the humans who log into a tenant's portal) carry a Roles\n    array set via POST /1.0/subscriptions/{SubscriptionID}/users and PUT\n    /1.0/subscriptions/{SubscriptionID}/users/{UserID}/roles. Those are end-user\n    portal roles, not API token scopes.\ngaps:\n- No OAuth 2.0 or OpenID Connect; /.well-known/oauth-authorization-server and\n  /.well-known/openid-configuration return 404 on exclaimer.com.\n- No documented token lifetime, expiry or rotation for the Cloud API token.\n- No scope model, so a partner token is all-or-nothing across every operation\n  including\
  \ destructive ones (end subscription, delete user, claim transfer).\nrelated_but_distinct:\n  name: Exclaimer Exchange Transport Agent API keys\n  docs: https://support.exclaimer.com/hc/en-gb/articles/12959044101277-API-Keys\n  note: >-\n    A separate mechanism. These keys authenticate an on-premises Exchange server\n    to the Exclaimer environment during Transport Agent installation, are managed\n    in the Exclaimer admin portal by an Exclaimer Administrator, and expire after\n    one year. They are NOT credentials for the Exclaimer Cloud API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/exclaimer/refs/heads/main/authentication/exclaimer-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Email
- Email Signatures
- Email Signature Management
- Microsoft-365
- Google Workspace
- Marketing
- Productivity
- Software-as-a-Service
- Security
---
