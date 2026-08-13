---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Digital Shadows Authentication
name_suffix: Authentication
oauth_flows: []
overview: Digital Shadows secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Digital Shadows
provider_slug: digital-shadows
scheme_count: 1
schemes:
- credentials:
  - issuance: Self-service inside the authenticated portal — the key and secret are read from Stored Objects > Portal > SearchLight API doc. Third-party integration guides (Sekoia, Axonius, ThreatConnect, Atlassian Marketplace) all instruct customers to retrieve the key and secret from that portal page.
    issued_by: SearchLight portal
    name: API key
  - issued_by: SearchLight portal
    name: API secret
  evidence: 'ds_base_service.DSBaseService builds base64.b64encode(f"{ds_api_key}:{ds_api_secret_key}") and sends it as ''Authorization: Basic <hash>''. shadowline''s SearchLightApi sets requests.Session().auth = (username, password), the equivalent Basic tuple.'
  in: header
  name: BasicAuth
  parameter: Authorization
  scheme: basic
  sources:
  - https://github.com/digitalshadows/splunk-soar-digitalshadows/blob/main/dsapi/service/ds_base_service.py
  - https://github.com/digitalshadows/shadowline-api/blob/master/shadowline/searchlight.py
  type: http
  value_form: Basic base64(<api_key>:<api_secret>)
slug: digital-shadows-authentication
source_filename: digital-shadows-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://github.com/digitalshadows/splunk-soar-digitalshadows/blob/main/dsapi/service/ds_base_service.py\ndocs: https://portal-digitalshadows.com/\ndocs_access: gated\ndocs_note: >-\n  The SearchLight API reference is published only inside the authenticated customer\n  portal (Stored Objects > Portal > SearchLight API doc). The auth model below is\n  read from Digital Shadows' own published client source, not from a public\n  reference page.\nsummary:\n  types: [http]\n  http_schemes: [basic]\n  api_key_in: []\n  oauth2_flows: []\n  oauth2: false\n  oidc: false\n  mtls: false\n  note: >-\n    No OAuth 2.0, OpenID Connect or mTLS surface. Credentials are a portal-issued\n    API key + secret used as HTTP Basic username + password. There is consequently\n    no scope surface, so scopes/ is deliberately not emitted.\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  in: header\n  parameter: Authorization\n  value_form:\
  \ 'Basic base64(<api_key>:<api_secret>)'\n  credentials:\n  - name: API key\n    issued_by: SearchLight portal\n    issuance: >-\n      Self-service inside the authenticated portal — the key and secret are read\n      from Stored Objects > Portal > SearchLight API doc. Third-party integration\n      guides (Sekoia, Axonius, ThreatConnect, Atlassian Marketplace) all instruct\n      customers to retrieve the key and secret from that portal page.\n  - name: API secret\n    issued_by: SearchLight portal\n  sources:\n  - https://github.com/digitalshadows/splunk-soar-digitalshadows/blob/main/dsapi/service/ds_base_service.py\n  - https://github.com/digitalshadows/shadowline-api/blob/master/shadowline/searchlight.py\n  evidence: >-\n    ds_base_service.DSBaseService builds\n    base64.b64encode(f\"{ds_api_key}:{ds_api_secret_key}\") and sends it as\n    'Authorization: Basic <hash>'. shadowline's SearchLightApi sets\n    requests.Session().auth = (username, password), the equivalent Basic tuple.\n\
  validation:\n  endpoint: /api/session-user\n  method: GET\n  description: >-\n    First-party credential check — DSBaseService.valid_credentials() calls\n    /api/session-user and treats a 2xx as valid credentials.\n  source: https://github.com/digitalshadows/splunk-soar-digitalshadows/blob/main/dsapi/service/ds_base_service.py\ntransport:\n  tls_required: true\n  observed_tls: TLSv1.3\n  see: security/digital-shadows-domain-security.yml\nx-evidence:\n- url: https://portal-digitalshadows.com/api/\n  http_status: 401\n  note: >-\n    Anonymous request returns {\"code\":\"PS491\",\"status\":401,\"message\":\"Failed to\n    authenticate, details are either incorrect (username and/or password) or the\n    account is locked/disabled...\"} — confirming credential-pair authentication.\n- url: https://raw.githubusercontent.com/digitalshadows/splunk-soar-digitalshadows/main/dsapi/service/ds_base_service.py\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digital-shadows/refs/heads/main/authentication/digital-shadows-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cybersecurity
- Threat Intelligence
- Digital Risk Protection
- Dark Web Monitoring
- Data Breach
- Brand Protection
- Security Operations
- Vulnerability Intelligence
---
