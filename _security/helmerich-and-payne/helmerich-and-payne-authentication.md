---
anonymous_access: false
api_key_in: []
api_specs:
- filename: helmerich-and-payne-survey-validation-controller-api-openapi.yml
  format: yaml
  label: Helmerich & Payne Survey Validation Controller API
  slug: helmerich-and-payne-survey-validation-controller-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/helmerich-and-payne/refs/heads/main/openapi/helmerich-and-payne-survey-validation-controller-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Helmerich And Payne Authentication
name_suffix: Authentication
oauth_flows: []
overview: Helmerich & Payne declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Helmerich & Payne
provider_slug: helmerich-and-payne
scheme_count: 0
schemes: []
slug: helmerich-and-payne-authentication
source_filename: helmerich-and-payne-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-13'\nmethod: probed\nsource: >-\n  openapi/helmerich-and-payne-magvar-survey-validation.json (harvested from\n  https://fac-api.magvar.com/v2/api-docs) plus a live unauthenticated call to\n  https://fac-api.magvar.com/uncertaintyValues on 2026-09-13.\nsummary: >-\n  There is no authentication. The MagVAR Survey Validation API declares no `securityDefinitions`\n  and no `security` block anywhere in its Swagger 2.0 contract, and a fully anonymous GET with the\n  spec's own default parameter values returned HTTP 200 with a complete result body. This is not an\n  undocumented-auth gap — it is an open, keyless, read-only public endpoint.\nschemes: []\nsecurity_applied: false\nanonymous_access:\n  verified: true\n  method: probed\n  probe:\n    url: https://fac-api.magvar.com/uncertaintyValues\n    request: GET with the 19 required query parameters at their spec-declared defaults\n    status: 200\n    content_type: application/json;charset=UTF-8\n    checked:\
  \ '2026-09-13'\n  note: >-\n    Returned a real computed result (sigmaValidation.distance 0.9495, three Green validation\n    results, inclination/azimuth uncertainties). No API key, header, cookie or token was sent.\nlicense_gate:\n  documented: true\n  url: https://www.magvar.com/EULA_SurveyValidationAPI.html\n  status: 200\n  note: >-\n    Access is technically open but legally licensed. The Survey Validation API EULA grants a\n    non-exclusive one-year single-user single-computer licence and explicitly contemplates both\n    paid and free licences; it prohibits redistribution, sublicensing and derivative works. There\n    is no technical enforcement point on the endpoint — the licence is the only gate. An agent\n    calling this API is inside a EULA it was never asked to accept, which is the honest risk to\n    record here.\naccount_surfaces:\n  - name: MagVAR / H&P customer login\n    url: https://www.hpinc.com/customer-login\n    status: 200\n    note: >-\n      The customer login\
  \ fronts Saphira (saphira.magvar.com) and the MagVAR account area. It is NOT\n      the gate for the Survey Validation API, which is anonymous.\ndocs:\n  - url: https://fac-api.magvar.com/swagger-ui.html\n    status: 200\n    note: Springfox Swagger UI 2.9.2; the only published API reference. It documents no auth step.\ngaps:\n  - No securitySchemes / securityDefinitions in the contract.\n  - No rate limiting, quota, or attribution mechanism is visible on an anonymous call, so the\n    provider has no way to tie usage to the EULA it publishes.\n  - No OAuth, OIDC or key-issuance surface exists on any H&P or MagVAR host (see\n    well-known/helmerich-and-payne-well-known.yml — all discovery paths 404).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/helmerich-and-payne/refs/heads/main/authentication/helmerich-and-payne-authentication.yml
summary_line: 0 schemes
tags:
- Oil and Gas
- Drilling
- Energy
- Wellbore Placement
- Directional Drilling
- Survey Management
- Geomagnetics
- Rig Automation
- Industrial
---
