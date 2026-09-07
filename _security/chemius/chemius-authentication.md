---
anonymous_access: false
api_key_in: []
auth_types: []
description: 'Authentication posture for the Chemius API estate, established by reading every public Chemius API page and probing every discovery path. The result is a measured absence: Chemius documents no authentication mechanism publicly. No API key, token, OAuth flow, mTLS or basic-auth scheme is named anywhere on the public site, and no reference is reachable without a sales call.'
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Chemius Authentication
name_suffix: Authentication
oauth_flows: []
overview: Chemius declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Chemius
provider_slug: chemius
scheme_count: 0
schemes: []
slug: chemius-authentication
source_filename: chemius-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Chemius\nproviderId: chemius\ngenerated: '2026-09-05'\nmethod: searched\nsource: >-\n  https://www.chemius.net/api/ and all seven per-API pages on www.chemius.net;\n  /.well-known/* probes on www.chemius.net, chemius.net, my.chemius.net, app.chemius.net\ndescription: >-\n  Authentication posture for the Chemius API estate, established by reading every public Chemius\n  API page and probing every discovery path. The result is a measured absence: Chemius documents no\n  authentication mechanism publicly. No API key, token, OAuth flow, mTLS or basic-auth scheme is\n  named anywhere on the public site, and no reference is reachable without a sales call.\ndocumented: false\nschemes: []\nschemes_note: >-\n  Zero securitySchemes can be derived, because no OpenAPI, WSDL or GraphQL SDL is published. Zero\n  can be searched, because every per-API page ends at \"Book a call & ask for the API documentation\"\
  \n  rather than at a reference.\nno_authentication_pointer_note: >-\n  No `type: Authentication` pointer is wired in apis.yml. The scorer's authentication_documented\n  check asserts the PROVIDER documents authentication; Chemius does not, and emitting the pointer\n  over this file would turn a recorded absence into a false claim.\ndiscovery_probes:\n  - url: https://www.chemius.net/.well-known/openid-configuration\n    status: 404\n  - url: https://www.chemius.net/.well-known/oauth-authorization-server\n    status: 404\n  - url: https://my.chemius.net/.well-known/oauth-authorization-server\n    status: 404\n  - url: https://my.chemius.net/.well-known/oauth-protected-resource\n    status: 404\n  - url: https://app.chemius.net/.well-known/openid-configuration\n    status: 404\nobserved_surface:\n  api_host_candidate: https://my.chemius.net/api\n  evidence:\n    - url: https://my.chemius.net/api/asset/image/e387e2e59f8b44e2c715d844a3b3c5ab.gif\n      status: 200\n      content_type: image/gif\n\
  \      note: >-\n        Referenced from the provider's own public page\n        https://www.chemius.net/chemius-api-integration-example/api-product1/ . An unauthenticated\n        GET returns the real asset, so at least one read path under /api/ is anonymous.\n    - url: https://my.chemius.net/api/\n      status: 404\n      note: >-\n        Returns a CodeIgniter \"404 Page Not Found\" router page, not the Angular SPA shell — which\n        is what establishes that a real API router lives at this path rather than a catch-all.\n  caveat: >-\n    This is the application's own backend, reached by the Chemius single-page app. Chemius does NOT\n    state it as the base URL of the seven commercial APIs, so it is recorded here as an observation\n    and deliberately NOT written into apis.yml baseURL. Guessing a base from an internal app route\n    is exactly the error this pipeline forbids.\naccount_authentication:\n  surface: https://my.chemius.net/login\n  method: email/username + password\n\
  \  mfa_documented: false\n  sso_documented: false\n  note: >-\n    Human sign-in to the Chemius application. Registration is self-serve and free\n    (https://my.chemius.net/register), but the pricing page states paid accounts are \"manually\n    reviewed\" before activation, so API-bearing accounts are not self-serve.\nprovisioning:\n  self_serve: false\n  path: >-\n    Buy a paid plan, then \"Request Add-on\" per API, then \"Book a call & ask for the API\n    documentation\". API credentials are issued through a sales and onboarding motion; no key is\n    obtainable from the website.\n  evidence: https://www.chemius.net/safety-data-sheet-api/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chemius/refs/heads/main/authentication/chemius-authentication.yml
summary_line: 0 schemes
tags:
- ADR
- Artificial Intelligence
- Chemicals
- Chemists
- Compliance
- GHS
- Hazard Communication
- Labels
- REACH
- Regulatory
- Research
- Safety Data Sheets
- Software-as-a-Service
- SDS
- TDS
---
