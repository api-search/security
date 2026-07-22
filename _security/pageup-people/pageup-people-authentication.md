---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Pageup People Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: PageUp People secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: PageUp People
provider_slug: pageup-people
scheme_count: 1
schemes:
- credentials_issued_by: PageUp (per-tenant, UAT then production)
  description: The PageUp API is secured with OAuth 2.0 client-credentials. Integration partners obtain OAuth 2.0 client credentials (client id + secret) from PageUp for the UAT (sandbox) environment first, then request production credentials from their PageUp Technical Consultant to go live. Per-tenant API domains and token endpoints are provisioned by PageUp for each client and are not published as a single public host.
  flow: clientCredentials
  name: OAuth2ClientCredentials
  sources:
  - docs
  type: oauth2
slug: pageup-people-authentication
source_filename: pageup-people-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://developers.pageuppeople.com/Content/getting-started\ndocs: https://developers.pageuppeople.com/Content/getting-started\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  description: >-\n    The PageUp API is secured with OAuth 2.0 client-credentials. Integration\n    partners obtain OAuth 2.0 client credentials (client id + secret) from PageUp\n    for the UAT (sandbox) environment first, then request production credentials\n    from their PageUp Technical Consultant to go live. Per-tenant API domains and\n    token endpoints are provisioned by PageUp for each client and are not\n    published as a single public host.\n  credentials_issued_by: PageUp (per-tenant, UAT then production)\n  sources:\n  - docs\nnotes: >-\n  No public OpenAPI/Swagger document is available (the developer portal at\n  developers.pageuppeople.com\
  \ is client/partner-facing), so this profile is\n  searched from the published getting-started documentation rather than derived\n  from a spec. OAuth scopes/permissions are not publicly documented; no scopes/\n  artifact is emitted.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pageup-people/refs/heads/main/authentication/pageup-people-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Talent Management
- Talent Acquisition
- Human Resources
- Recruiting
- Applicant Tracking
- Onboarding
- Learning
- HR Technology
- SaaS
---
