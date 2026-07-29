---
api_key_in: []
api_specs:
- filename: uk-caa-consultations-api-openapi.yml
  format: yaml
  label: CAA Consultations API
  slug: caa-consultations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uk-caa/refs/heads/main/openapi/uk-caa-consultations-api-openapi.yml
auth_types:
- none
description: 'Authentication profile for every UK Civil Aviation Authority API surface that was probed. The one documented, publicly callable API on a caa.co.uk domain — the Citizen Space consultations API — requires NO authentication at all. That is a documented posture, not an omission: the vendor developer guide the CAA links to states verbatim that "the current version of the API provides read-only access to publicly visible data. This means that no authentication is required as the access level is the same as a public visitor to the site." The remaining CAA surfaces are gated by mechanisms that are not developer authentication (browser-origin locking, reCAPTCHA, ADFS WS-Federation employee/licence-holder sign-in, or a paid order form).'
kind: authentication
layout: security
method: searched
name: Uk Caa Authentication
name_suffix: Authentication
oauth_flows: []
overview: UK Civil Aviation Authority secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: UK Civil Aviation Authority
provider_slug: uk-caa
scheme_count: 0
schemes: []
slug: uk-caa-authentication
source_filename: uk-caa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: >-\n  https://consultations.caa.co.uk/api/2.4/ and\n  https://help.delib.net/article/350-api-v2-x-developers-guide (the vendor guide the\n  CAA's own API reference links to), plus a live anonymous request verified\n  2026-07-28.\ndocs: https://help.delib.net/article/350-api-v2-x-developers-guide\ndescription: >-\n  Authentication profile for every UK Civil Aviation Authority API surface that was\n  probed. The one documented, publicly callable API on a caa.co.uk domain — the\n  Citizen Space consultations API — requires NO authentication at all. That is a\n  documented posture, not an omission: the vendor developer guide the CAA links to\n  states verbatim that \"the current version of the API provides read-only access to\n  publicly visible data. This means that no authentication is required as the access\n  level is the same as a public visitor to the site.\" The remaining CAA surfaces are\n  gated by mechanisms that are\
  \ not developer authentication (browser-origin locking,\n  reCAPTCHA, ADFS WS-Federation employee/licence-holder sign-in, or a paid order\n  form).\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The OpenAPI carries no securitySchemes because the API genuinely declares none.\n    derive-authentication.py therefore produced no profile; this file was written\n    from the published documentation instead.\nschemes: []\nsurfaces:\n  - name: CAA Consultations API (Citizen Space 2.4)\n    base_url: https://consultations.caa.co.uk/api/2.4\n    auth: none\n    verified: '2026-07-28'\n    evidence: >-\n      Anonymous GET /api/2.4/json_search_results?st=open&fields=all returned HTTP\n      200, application/json, 57,395 bytes with no key, no header, no cookie and no\n      signup. Response headers include access-control-allow-origin: * — the API is\n      callable directly from a browser on any origin.\n    transport_security:\n      https: true\n      hsts: true\n\
  \      hsts_max_age: 31536000\n      cors: '*'\n    read_only: true\n    docs: https://consultations.caa.co.uk/api/2.4/\n  - name: G-INFO aircraft register search backend\n    base_url: https://ginfoapi.caa.co.uk/api/aircraft\n    auth: none-published\n    gate: browser-origin\n    evidence: >-\n      Undocumented internal backend for the CAA's own G-INFO search widget. GET\n      returns 405; an unauthenticated POST returns 400 with response header\n      access-control-allow-origin: https://www.caa.co.uk. There is no published\n      credential a developer can obtain — this is origin pinning, not authentication.\n  - name: Check an ATOL search backend\n    base_url: https://aircraftapi.caa.co.uk/api/checkanatol\n    auth: none-published\n    gate: browser-origin + reCAPTCHA\n    evidence: >-\n      Undocumented internal backend for the Check an ATOL widget. GET returns 405,\n      unauthenticated POST returns 400, origin-locked to https://www.caa.co.uk, and\n      the host page carries\
  \ a data-recaptchasitekey attribute.\n  - name: CAA Customer Portal\n    base_url: https://portal.caa.co.uk\n    auth: ws-federation\n    idp: https://sso.caa.co.uk\n    evidence: >-\n      portal.caa.co.uk redirects to an ADFS WS-Federation sign-in at sso.caa.co.uk.\n      This is a licence/certificate-holder login, not a developer credential; no\n      OIDC discovery document is served (/.well-known/openid-configuration -> 404).\n  - name: Bulk G-INFO aircraft register\n    auth: commercial\n    evidence: >-\n      Paid subscription ordered on a form and emailed as an MS Excel file, licensed\n      for use on a single PC. A commercial agreement, not an API credential.\ngaps:\n  - No API key programme, no OAuth 2.0 authorization server, no OIDC discovery, and\n    no mTLS on any CAA API host.\n  - No published API terms of service, rate-limit policy or SLA for the one\n    documented API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uk-caa/refs/heads/main/authentication/uk-caa-authentication.yml
summary_line: none · 0 schemes
tags:
- Travel
- United Kingdom
- Aviation
- Airline
- Airports
- Regulator
- Government
- Distribution
- Consumer Protection
- Open Data
---
