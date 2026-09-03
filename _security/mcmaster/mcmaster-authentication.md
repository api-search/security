---
api_key_in: []
api_specs:
- filename: mcmaster-experts-openapi.yml
  format: yaml
  label: McMaster Experts API
  slug: experts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcmaster/refs/heads/main/openapi/mcmaster-experts-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Mcmaster Authentication
name_suffix: Authentication
oauth_flows: []
overview: McMaster University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: McMaster University
provider_slug: mcmaster
scheme_count: 0
schemes: []
slug: mcmaster-authentication
source_filename: mcmaster-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# x-method is the AUTHORSHIP vocabulary build-provenance-manifest.py reads (who wrote the\n# file: we did). `method: probed` below is the university-pipeline PROVENANCE vocabulary\n# (how we came to hold it: live probe). Two axes, two keys, neither guessed.\nx-method: generated\nversion: '0.1'\ngenerated: '2026-09-01'\nmethod: probed\nsource: https://experts.mcmaster.ca/api/people\nnote: >-\n  Authentication posture per surface, established by probing on 2026-09-01. McMaster operates two\n  very different doors: a gated Azure API Management portal that nothing can be read through, and an\n  undocumented anonymous JSON API that anyone can read everything through.\nsurfaces:\n  - surface: McMaster Experts API\n    host: experts.mcmaster.ca\n    x-operator: institution\n    scheme: none\n    detail: >-\n      No authentication of any kind. /api/search, /api/people and /api/publications each answer\n      anonymously over HTTPS with no key, cookie, Origin restriction or Referer\
  \ check. No\n      WWW-Authenticate, no 401 path, no securitySchemes.\n    evidence:\n      - url: https://experts.mcmaster.ca/api/people\n        status: 200\n      - url: https://experts.mcmaster.ca/api/publications\n        status: 200\n    caveat: >-\n      Anonymous access to 7,301 person records carrying macid values is a disclosure worth naming.\n      See review.yml. It is not presented here as a feature.\n  - surface: McMaster API Service Developer Portal\n    host: developer.api.mcmaster.ca\n    x-operator: institution\n    scheme: institutional_sso\n    detail: >-\n      Azure API Management developer portal. Both /apis and /products 302 to\n      /signin?returnUrl=..., so neither the API catalog nor the product list can be read\n      anonymously. Sign-in requires a MacID plus a registration step. No anonymous OpenAPI, no\n      public product list, no published terms.\n    evidence:\n      - url: https://developer.api.mcmaster.ca/apis\n        status: 200\n        locator:\
  \ redirected to https://developer.api.mcmaster.ca/signin?returnUrl=%2Fapis\n      - url: https://developer.api.mcmaster.ca/products\n        status: 200\n        locator: redirected to https://developer.api.mcmaster.ca/signin?returnUrl=%2Fproducts\n  - surface: MacSphere DSpace REST + OAI-PMH\n    host: macsphere.mcmaster.ca\n    x-operator: institution\n    scheme: none_for_read\n    detail: >-\n      Read operations are anonymous. DSpace 8.2 exposes /server/api/authn for authenticated write\n      and submission workflows, which are not public. OAI-PMH is fully anonymous.\n    evidence:\n      - url: https://macsphere.mcmaster.ca/server/api\n        status: 200\n        locator: _links.authn -> /server/api/authn\n  - surface: McMaster Shibboleth IdP\n    host: sso.mcmaster.ca\n    x-operator: federation\n    scheme: saml2_shibboleth\n    detail: >-\n      This surface IS McMaster's authentication. The IdP metadata document is anonymous and\n      machine-readable; the SSO profile endpoint\
  \ requires a valid SAML AuthnRequest (a bare GET\n      returns 400). The host root returns 403, which is correct hardening, not a fault.\n    evidence:\n      - url: https://sso.mcmaster.ca/idp/shibboleth\n        status: 200\n      - url: https://sso.mcmaster.ca/idp/profile/SAML2/Redirect/SSO\n        status: 400\n      - url: https://sso.mcmaster.ca/\n        status: 403\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcmaster/refs/heads/main/authentication/mcmaster-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Canada
- Ontario
- U15 Group of Canadian Research Universities
- Research
- Research Data
- Research Repository
- Identity Federation
- Scholarly Communication
- Open Access
- Library
- Course Catalog
---
