---
api_key_in: []
api_specs:
- filename: oracle-health-data-intelligence-populations-api-openapi.yml
  format: yaml
  label: Oracle Health Data Intelligence Populations API
  slug: oracle-health-data-intelligence-populations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-health-data-intelligence/refs/heads/main/openapi/oracle-health-data-intelligence-populations-api-openapi.yml
auth_types:
- http
- oauth1
description: Authentication profile for the Oracle Health Data Intelligence (formerly Cerner HealtheIntent) APIs, read from the provider's own developer-portal Getting Started section and confirmed against a live unauthenticated request to the demo tenant.
kind: authentication
layout: security
method: searched
name: Oracle Health Data Intelligence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle Health Data Intelligence secures its APIs with http and oauth1 across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Oracle Health Data Intelligence
provider_slug: oracle-health-data-intelligence
scheme_count: 2
schemes:
- description: Bearer token issued to an Oracle system account, sent in the Authorization header. Oracle calls this the simpler and recommended method.
  name: bearerAuth
  preferred: true
  scheme: bearer
  sources:
  - https://docs.healtheintent.com/#authenticating-using-a-bearer-token
  - openapi/oracle-health-data-intelligence-populations-api-openapi.yml
  token_lifetime: Does not expire automatically. Oracle instructs customers to rotate the bearer token manually on a regular schedule, when an administrator account is removed, and on any suspicion of compromise.
  type: http
- credentials:
  - consumer key
  - consumer secret
  description: Two-legged OAuth 1.0a using a consumer key and consumer secret issued with the system account. The consumer credentials are exchanged for a short-lived oauth_token used in an OAuth Authorization header. Documented as the alternative to bearer.
  flow: two-legged
  name: oauth1
  preferred: false
  sources:
  - https://docs.healtheintent.com/#authenticating-using-oauth
  spec: https://oauth.net/core/1.0a/
  token_lifetime: oauth_expires_in 3600 seconds; oauth_authorization_expires_in 86400 seconds
  type: oauth1
  vendor_spec: https://wiki.ucern.com/x/MgTJRg
  version: 1.0a
slug: oracle-health-data-intelligence-authentication
source_filename: oracle-health-data-intelligence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://docs.healtheintent.com/#authentication\ndocs: https://docs.healtheintent.com/#authentication\ndescription: >-\n  Authentication profile for the Oracle Health Data Intelligence (formerly Cerner HealtheIntent)\n  APIs, read from the provider's own developer-portal Getting Started section and confirmed against\n  a live unauthenticated request to the demo tenant.\nsummary:\n  types:\n    - http\n    - oauth1\n  preferred: bearer\n  identity_model: system-account\n  user_level_authorization: false\n  self_serve: false\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    preferred: true\n    description: >-\n      Bearer token issued to an Oracle system account, sent in the Authorization header. Oracle\n      calls this the simpler and recommended method.\n    token_lifetime: >-\n      Does not expire automatically. Oracle instructs customers to rotate the bearer token manually\n      on a regular schedule,\
  \ when an administrator account is removed, and on any suspicion of\n      compromise.\n    sources:\n      - https://docs.healtheintent.com/#authenticating-using-a-bearer-token\n      - openapi/oracle-health-data-intelligence-populations-api-openapi.yml\n  - name: oauth1\n    type: oauth1\n    version: 1.0a\n    flow: two-legged\n    preferred: false\n    description: >-\n      Two-legged OAuth 1.0a using a consumer key and consumer secret issued with the system\n      account. The consumer credentials are exchanged for a short-lived oauth_token used in an\n      OAuth Authorization header. Documented as the alternative to bearer.\n    credentials:\n      - consumer key\n      - consumer secret\n    token_lifetime: oauth_expires_in 3600 seconds; oauth_authorization_expires_in 86400 seconds\n    spec: https://oauth.net/core/1.0a/\n    vendor_spec: https://wiki.ucern.com/x/MgTJRg\n    sources:\n      - https://docs.healtheintent.com/#authenticating-using-oauth\nonboarding:\n  self_serve:\
  \ false\n  process: >-\n    A system account must be requested through the Cerner Central portal (US or EU), naming the\n    customer, the solution, an Oracle contact and the environment. Once approved, an administrator\n    must additionally grant that system account authorization for each API and resource in the\n    Health Data Intelligence Console.\n  request_portals:\n    - region: US\n      url: https://cernercentral.com/system-accounts/\n    - region: EU\n      url: https://eu.cernercentral.com/system-accounts/\n  authorization_step: Health Data Intelligence Console, per API and per resource\n  note: >-\n    Access is customer-scoped. There is no public signup, no free tier and no anonymous key. The\n    APIs are B2B and, in Oracle's own words, \"user-level authorization and filtering are not\n    applied\" — the calling system is responsible for applying user authorization.\nx-evidence:\n  fetched: '2026-08-27'\n  url: https://cernerdemo.api.us-1.healtheintent.com/allergy/v1/populations/{populationId}/patients/{patientId}/allergies\n\
  \  http_status: 401\n  www_authenticate: >-\n    Bearer realm=cernerdemo.api.us-1.healtheintent.com OAuth realm=cernerdemo.api.us-1.healtheintent.com\n  note: >-\n    The live WWW-Authenticate header advertises both Bearer and OAuth challenges on the same\n    resource, independently confirming the dual scheme documented above.\nscopes:\n  applicable: false\n  reason: >-\n    No OAuth 2.0 surface exists, so there is no scope vocabulary. Authorization is granted per API\n    and per resource to a system account in the Health Data Intelligence Console, out of band from\n    the token. scopes/ is deliberately not emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-health-data-intelligence/refs/heads/main/authentication/oracle-health-data-intelligence-authentication.yml
summary_line: http/oauth1 · 2 schemes
tags:
- Genomic
- Health Records
- Healthcare
- Population Health
- Longitudinal Record
- Interoperability
- Clinical Data
- Analytics
---
