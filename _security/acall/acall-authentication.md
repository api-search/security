---
anonymous_access: false
api_key_in: []
api_specs:
- filename: acall-public-api-openapi.yml
  format: yaml
  label: Acall Public API
  slug: acall-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acall/refs/heads/main/openapi/acall-public-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Acall Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acall secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Acall
provider_slug: acall
scheme_count: 1
schemes:
- applied: global
  description: Access token for API
  name: Bearer
  note: 'Declared as a document-level security requirement (security: [{Bearer: []}]) in the Acall Public API spec, so it applies to all 13 operations.'
  scheme: bearer
  sources:
  - openapi/acall-public-api-openapi.yml
  type: http
slug: acall-authentication
source_filename: acall-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: openapi/acall-public-api-openapi.yml\ndocs: https://support.workstyleos.com/faq/show/598?site_domain=default\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  description: Access token for API\n  sources:\n  - openapi/acall-public-api-openapi.yml\n  applied: global\n  note: >-\n    Declared as a document-level security requirement (security: [{Bearer: []}]) in the Acall Public API\n    spec, so it applies to all 13 operations.\ncredential_issuance:\n  self_serve: false\n  process: >-\n    Acall does not issue API tokens through a developer console. The published help-centre article\n    \"利用できる API を教えてください\" (FAQ 598) instructs customers to submit the contact form with\n    「API利用希望」 (request to use the API) in the body; Acall reviews the request and then issues an\n    access token by reply.\n  request_url: https://support.workstyleos.com/faq/show/1250?site_domain=default\n\
  \  restrictions:\n  - >-\n    The API is not available to customers on the multi-tenant (マルチテナント) plan — stated verbatim in\n    FAQ 598 under ご利用条件.\n  source: https://support.workstyleos.com/faq/show/598?site_domain=default\nobserved_challenge:\n  probed: '2026-09-06'\n  note: >-\n    Live unauthenticated probes of the production base URL return an RFC 6750 bearer challenge. Bodies are\n    text/plain, not JSON.\n  probes:\n  - url: https://api.workstyleos.com/v1/users\n    request: no Authorization header\n    status: 401\n    www_authenticate: Bearer realm=\"token_required\"\n    body: Unauthenticated\n  - url: https://api.workstyleos.com/v1/users\n    request: \"Authorization: Bearer <invalid>\"\n    status: 401\n    www_authenticate: Bearer error=\"invalid_token\"\n    body: Unauthenticated\n  - url: https://api.workstyleos.com/v1/nope\n    request: no Authorization header\n    status: 404\n    www_authenticate: Bearer error=\"not_found\"\n    body: Not found endpoint\nsso:\n  note:\
  \ >-\n    Distinct from API authentication: the Acall Portal end-user product supports SAML/OIDC single sign-on\n    (Microsoft Entra ID / Azure AD and others) as a paid option, and since the 2026-07-09 release supports\n    multiple simultaneous IdPs. This governs human login to portal.workstyleos.com, not Public API tokens.\n  source: https://www.workstyleos.com/security/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acall/refs/heads/main/authentication/acall-authentication.yml
summary_line: http · 1 scheme
tags:
- Workplace Management
- Visitor Management
- Meeting Room Booking
- Desk Booking
- Hybrid Work
- Access Control
- Facilities
- Smart Office
- Japan
- SaaS
---
