---
api_key_in: []
api_specs:
- filename: hbku-fanar-api-openapi.yml
  format: yaml
  label: Fanar API
  slug: fanar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-fanar-api-openapi.yml
- filename: hbku-farasa-api-openapi.yml
  format: yaml
  label: Farasa Web API
  slug: farasa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/openapi/hbku-farasa-api-openapi.yml
auth_types:
- http-bearer
- api-key-in-body
description: Authentication across the two APIs Hamad Bin Khalifa University actually operates. Both are key-based and both require registration; neither offers OAuth, and neither publishes a scope vocabulary, so this repository carries no scopes/ artifact. This file replaces an earlier one derived from Figshare's OAuth contract, which described a vendor's authentication scheme and not the university's.
kind: authentication
layout: security
method: derived
name: Hbku Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hamad Bin Khalifa University secures its APIs with http-bearer and api-key-in-body across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Hamad Bin Khalifa University
provider_slug: hbku
scheme_count: 2
schemes:
- api: Fanar API
  description: '"Provide your API key in the Authorization header using the Bearer scheme." Declared at components.securitySchemes.Bearer and applied document-wide via a root security requirement, so every one of the 12 operations is authenticated.'
  in: header
  name: Bearer
  parameter: Authorization
  registration: https://api.fanar.qa/request/en
  scheme: bearer
  sources:
  - openapi/_original/hbku-fanar-api-openapi.json
  type: http
  verified:
    body: '{"error":{"code":"invalid_authentication","message":"Invalid authentication","status":401}}'
    date: '2026-08-30'
    probe: GET https://api.fanar.qa/v1/models
    status: 401
  x-operator: institution
- api: Farasa Web API
  description: Farasa carries its key as a body field alongside the text, in both the JSON and the form-encoded variants. This is the provider's own documented pattern, taken from the Python, Java, JavaScript and curl samples published on each module page — not a reconstruction.
  in: body
  name: api_key
  parameter: api_key
  registration: https://farasa.qcri.org/
  sources:
  - https://farasa.qcri.org/lemmatization/
  type: apiKey
  verified:
    body: 'invalid api key. please register at: https://farasa.qcri.org'
    date: '2026-08-30'
    probe: POST https://farasa.qcri.org/webapi/lemmatization/
    status: 400
  x-operator: institution
slug: hbku-authentication
source_filename: hbku-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: derived\nsource:\n- openapi/_original/hbku-fanar-api-openapi.json\n- openapi/hbku-farasa-api-openapi.yml\nprovider: Hamad Bin Khalifa University\nproviderId: hbku\ndescription: >-\n  Authentication across the two APIs Hamad Bin Khalifa University actually operates. Both are\n  key-based and both require registration; neither offers OAuth, and neither publishes a scope\n  vocabulary, so this repository carries no scopes/ artifact. This file replaces an earlier one\n  derived from Figshare's OAuth contract, which described a vendor's authentication scheme and not\n  the university's.\nsummary:\n  types:\n  - http-bearer\n  - api-key-in-body\n  oauth2_flows: []\n  scopes_published: false\nschemes:\n- name: Bearer\n  api: Fanar API\n  x-operator: institution\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  description: >-\n    \"Provide your API key in the Authorization header using the Bearer scheme.\" Declared at\n\
  \    components.securitySchemes.Bearer and applied document-wide via a root security requirement, so\n    every one of the 12 operations is authenticated.\n  registration: https://api.fanar.qa/request/en\n  verified:\n    probe: GET https://api.fanar.qa/v1/models\n    status: 401\n    body: '{\"error\":{\"code\":\"invalid_authentication\",\"message\":\"Invalid authentication\",\"status\":401}}'\n    date: '2026-08-30'\n  sources:\n  - openapi/_original/hbku-fanar-api-openapi.json\n- name: api_key\n  api: Farasa Web API\n  x-operator: institution\n  type: apiKey\n  in: body\n  parameter: api_key\n  description: >-\n    Farasa carries its key as a body field alongside the text, in both the JSON and the\n    form-encoded variants. This is the provider's own documented pattern, taken from the Python,\n    Java, JavaScript and curl samples published on each module page — not a reconstruction.\n  registration: https://farasa.qcri.org/\n  verified:\n    probe: POST https://farasa.qcri.org/webapi/lemmatization/\n\
  \    status: 400\n    body: 'invalid api key. please register at: https://farasa.qcri.org'\n    date: '2026-08-30'\n  sources:\n  - https://farasa.qcri.org/lemmatization/\nnotes: >-\n  HBKU publishes no institutional identity-federation surface. It is not registered in eduGAIN\n  (technical.edugain.org holds no Qatari federation and no hbku.edu.qa entity, checked 2026-08-30),\n  idp.hbku.edu.qa does not resolve, and sso.hbku.edu.qa presents a certificate that does not match\n  the hostname. So there is no IdentityFederation pointer to record.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hbku/refs/heads/main/authentication/hbku-authentication.yml
summary_line: http-bearer/api-key-in-body · 2 schemes
tags:
- University
- Higher Education
- Education
- Research
- Qatar
- Middle East
- Artificial Intelligence
- Large Language Models
- Natural Language Processing
- Arabic
- Research Computing
- Research Data
- Course Catalog
- Repository
- Open Access
---
