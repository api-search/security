---
anonymous_access: false
api_key_in: []
api_specs:
- filename: overview
  format: yaml
  label: 10x Banking Platform API
  slug: 10x-banking-platform-api
  spec_type: Postman
  url: https://www.postman.com/openbanking10x/10x-banking-public-workspace/overview
auth_types: []
description: 'The 10x platform API is fully authenticated at the edge: every path, routed or not, returns 401 to an anonymous caller. The scheme itself is not disclosed publicly. No WWW-Authenticate challenge is returned, no OAuth or OpenID discovery document is served on any 10x host, and the authentication guide is behind the ReadMe login.'
kind: authentication
layout: security
mechanism_count: 1
method: probed
name: 10X Banking Technology Services Authentication
name_suffix: Authentication
oauth_flows: []
overview: 10x Banking Technology Services declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: 10x Banking Technology Services
provider_slug: 10x-banking-technology-services
scheme_count: 1
schemes:
- confidence: low
  evidence:
  - https://api.sandbox.10xbanking.com/ returns HTTP 401 with body {"ref":"...","status":401,"code":"401.002.001","message":"Authentication is required to access this resource."} and NO WWW-Authenticate response header, so the scheme is not advertised per RFC 7235.
  - 10x's public Postman environment "10x Banking" carries an `apiKey` variable (empty, for the consumer to fill) next to baseUrl https://api.sandbox.10xbanking.com — first-party evidence pointing at an API-key or token credential the tenant is issued, but the header or parameter name it binds to is not published.
  id: undisclosed
  note: 'NOT recorded as apiKey. The Postman variable name is suggestive, not dispositive: the environment ships no collection, so nothing shows where the value is placed. Asserting a concrete scheme from a variable name would be a guess.'
  type: unknown
slug: 10x-banking-technology-services-authentication
source_filename: 10x-banking-technology-services-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  Live probes of https://api.sandbox.10xbanking.com plus 10x Banking's own public\n  Postman environment (https://www.postman.com/openbanking10x/10x-banking-public-workspace),\n  which declares an `apiKey` variable alongside the sandbox `baseUrl`. No OpenAPI\n  securitySchemes block was available to derive from — 10x publishes no spec.\ndescription: >-\n  The 10x platform API is fully authenticated at the edge: every path, routed or not,\n  returns 401 to an anonymous caller. The scheme itself is not disclosed publicly. No\n  WWW-Authenticate challenge is returned, no OAuth or OpenID discovery document is\n  served on any 10x host, and the authentication guide is behind the ReadMe login.\n\nstatus: gated\npublic_documentation: false\ndocs: https://docs.10xbanking.com/\ndocs_status: 302 to https://dash.readme.com/to/docs-10xbanking (login gate)\n\nschemes:\n  - id: undisclosed\n    type: unknown\n    confidence: low\n    evidence:\n\
  \      - >-\n        https://api.sandbox.10xbanking.com/ returns HTTP 401 with body\n        {\"ref\":\"...\",\"status\":401,\"code\":\"401.002.001\",\"message\":\"Authentication is\n        required to access this resource.\"} and NO WWW-Authenticate response header, so\n        the scheme is not advertised per RFC 7235.\n      - >-\n        10x's public Postman environment \"10x Banking\" carries an `apiKey` variable\n        (empty, for the consumer to fill) next to baseUrl\n        https://api.sandbox.10xbanking.com — first-party evidence pointing at an API-key\n        or token credential the tenant is issued, but the header or parameter name it\n        binds to is not published.\n    note: >-\n      NOT recorded as apiKey. The Postman variable name is suggestive, not dispositive:\n      the environment ships no collection, so nothing shows where the value is placed.\n      Asserting a concrete scheme from a variable name would be a guess.\n\ndiscovery:\n  openid_configuration: not\
  \ served (404 on marketing hosts, 401 on the API host)\n  oauth_authorization_server: not served (404 on marketing hosts, 401 on the API host)\n  oauth_protected_resource: not served (401 on the API host)\n  www_authenticate_header: absent\n\nkey_issuance:\n  self_service: false\n  mechanism: >-\n    Credentials are issued to tenants under a platform agreement. The public entry\n    points are https://www.10xbanking.com/book-a-demo and the platform evaluation\n    agreement at https://www.10xbanking.com/platform-evaluation-agreement. There is no\n    public sign-up, free tier, or key-generation console.\n\noauth2:\n  declared: false\n  note: >-\n    No oauth2 securityScheme could be read (no spec) and no OAuth metadata document is\n    served, so no scopes artifact is written. An absent scopes file here means \"not\n    published\", not \"no scopes exist\".\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/10x-banking-technology-services/refs/heads/main/authentication/10x-banking-technology-services-authentication.yml
summary_line: 1 scheme
tags:
- Financial-Services
- Banking
- Core Banking
- Cloud Native
- Banking as a Service
- Embedded Finance
- Payments
- Lending
- Deposits
- Cards
- Event Driven
- United Kingdom
- SaaS
- Fintech
---
