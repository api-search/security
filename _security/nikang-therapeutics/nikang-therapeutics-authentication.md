---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Nikang Therapeutics Authentication
name_suffix: Authentication
oauth_flows: []
overview: NiKang Therapeutics declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: NiKang Therapeutics
provider_slug: nikang-therapeutics
scheme_count: 0
schemes: []
slug: nikang-therapeutics-authentication
source_filename: nikang-therapeutics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  The `authentication` array in the WordPress REST index at https://www.nikangtx.com/wp-json (empty),\n  plus live anonymous requests against every route family on 2026-08-26. 0-working/derive-authentication.py\n  was run first and correctly found zero securitySchemes, because there are none to find — this file\n  records what was observed at the wire instead.\ndocs: https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/\nnote: >-\n  NiKang Therapeutics issues no API credentials of any kind. There is no developer portal, no signup,\n  no key request form and no OAuth client registration. The catalogued surface is anonymous read-only\n  content; authentication exists on this deployment only as the wall that separates that public\n  content from the WordPress administration surface, and there is no public path to get past it.\nschemes: []\nprofile:\n  style: none\n  anonymous_access: true\n  credentials_available_to_the_public:\
  \ false\n  detail: >-\n    The /wp-json index reports `\"authentication\": []` — no scheme is advertised for anonymous\n    discovery. Every read operation described in openapi/ was executed with no credentials and no\n    cookie and returned HTTP 200.\n  cors:\n    access_control_allow_headers: 'Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type'\n    detail: >-\n      The CORS preflight allow-list names `Authorization` and `X-WP-Nonce`, which is WordPress core\n      boilerplate advertising the schemes core would accept if a credential existed. It is not an\n      offer of credentials to the public and must not be read as one.\ngated_surface:\n  detail: >-\n    These routes are registered and visible in the public route index but return 401 anonymously.\n    They are excluded from openapi/ and are recorded here so the boundary is explicit.\n  observed:\n  - path: /wp/v2/users\n    status: 401\n    code: rest_user_cannot_view\n  - path: /wp/v2/settings\n    status:\
  \ 401\n    code: rest_forbidden\n  - path: /wp/v2/block-types\n    status: 401\n    code: rest_block_type_cannot_view\n  - path: /wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n  - path: /wp-site-health/v1/tests/background-updates\n    status: 401\n    code: rest_forbidden\n  - path: /oembed/1.0/proxy\n    status: 401\n    code: rest_forbidden\n  consequence: >-\n    /wp/v2/users being 401-gated is the one gap that matters for a consumer: posts carry an integer\n    `author` id that cannot be resolved to a name without credentials. Author display data is only\n    reachable indirectly, and the dt_team collection — not the users collection — is where NiKang's\n    named people actually live.\nwrite_surface:\n  anonymous: none\n  detail: >-\n    POST, PUT, PATCH and DELETE are registered on the post-like and term routes but every one of them\n    requires an authenticated user with the matching capability. There is no anonymous write path at\n    all, which is why\
  \ reversibility, dry-run and idempotency are all `na` in\n    conventions/nikang-therapeutics-conventions.yml.\ncross_links:\n  conventions: conventions/nikang-therapeutics-conventions.yml\n  errors: errors/nikang-therapeutics-problem-types.yml\n  scopes: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nikang-therapeutics/refs/heads/main/authentication/nikang-therapeutics-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Oncology
- Precision Medicine
- Drug Discovery
- Targeted Protein Degradation
- Clinical Trials
- Life Sciences
- content-api
---
