---
anonymous_access: false
api_key_in: []
api_specs:
- filename: postman-collection
  format: yaml
  label: Cloudability API v3
  slug: api-v3
  spec_type: Postman
  url: https://github.com/IBM/Apptio-Tools/tree/main/cloudability/postman-collection
auth_types: []
description: 'The Cloudability v3 API accepts two published credential styles. Neither is OAuth: there is no authorization server, no scopes document and no /.well-known/oauth-authorization-server on any host. Derivation from a spec was not possible — Cloudability publishes no OpenAPI — so this profile is read directly from IBM''s own getting-started page and confirmed against the live 401 the API returns.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Cloudability Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudability declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Cloudability
provider_slug: cloudability
scheme_count: 2
schemes:
- availability: All commercial regions. NOT supported in US GovCloud (api.usgov.cloudability.com) — that environment requires apptio-opentoken.
  description: 'A Cloudability API key used as HTTP Basic credentials. IBM''s documentation writes the header as `Authorization: Basic <cldy_token>`; the token is generated per user from the Cloudability preferences screen.'
  format: 'Authorization: Basic <cldy_token>'
  id: cloudability-api-key
  in: header
  key_provisioning: https://app.apptio.com/cloudability#/settings/preferences
  name: Authorization
  rotation: not documented
  scheme: basic
  type: http
- availability: All environments, including US GovCloud.
  companion_header:
    description: The Apptio environment id the request is scoped to.
    name: apptio-environmentid
    required: true
  description: 'The Apptio platform token, obtained from the Apptio Frontdoor Access Administration API. This is the only credential accepted in every environment including US GovCloud, and it is the direction of travel: IBM documents that user CRUD has already moved from the Cloudability v3 Users endpoint to the Apptio Frontdoor API.'
  id: apptio-opentoken
  in: header
  name: apptio-opentoken
  rotation: not documented
  type: apiKey
slug: cloudability-authentication
source_filename: cloudability-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: Cloudability\nproviderId: cloudability\ngenerated: '2026-09-05'\nmodified: '2026-09-05'\nmethod: searched\nsource: >-\n  https://www.ibm.com/docs/en/cloudability-commercial/cloudability-premium/saas?topic=api-getting-started-cloudability-v3\n  (\"Getting started with Cloudability API V3\") plus a live unauthenticated probe\n  of https://api.cloudability.com/v3 on 2026-09-05.\ndescription: >-\n  The Cloudability v3 API accepts two published credential styles. Neither is\n  OAuth: there is no authorization server, no scopes document and no\n  /.well-known/oauth-authorization-server on any host. Derivation from a spec was\n  not possible — Cloudability publishes no OpenAPI — so this profile is read\n  directly from IBM's own getting-started page and confirmed against the live\n  401 the API returns.\nschemes:\n  - id: cloudability-api-key\n    type: http\n    scheme: basic\n    in: header\n    name:\
  \ Authorization\n    format: 'Authorization: Basic <cldy_token>'\n    description: >-\n      A Cloudability API key used as HTTP Basic credentials. IBM's documentation\n      writes the header as `Authorization: Basic <cldy_token>`; the token is\n      generated per user from the Cloudability preferences screen.\n    key_provisioning: https://app.apptio.com/cloudability#/settings/preferences\n    availability: >-\n      All commercial regions. NOT supported in US GovCloud\n      (api.usgov.cloudability.com) — that environment requires apptio-opentoken.\n    rotation: not documented\n  - id: apptio-opentoken\n    type: apiKey\n    in: header\n    name: apptio-opentoken\n    companion_header:\n      name: apptio-environmentid\n      required: true\n      description: The Apptio environment id the request is scoped to.\n    description: >-\n      The Apptio platform token, obtained from the Apptio Frontdoor Access\n      Administration API. This is the only credential accepted in every\n\
  \      environment including US GovCloud, and it is the direction of travel: IBM\n      documents that user CRUD has already moved from the Cloudability v3 Users\n      endpoint to the Apptio Frontdoor API.\n    availability: All environments, including US GovCloud.\n    rotation: not documented\noauth:\n  supported: false\n  evidence:\n    - url: https://api.cloudability.com/.well-known/oauth-authorization-server\n      status: 401\n      note: blanket 401 on every path including a nonexistent control path\n    - url: https://www.ibm.com/.well-known/oauth-authorization-server\n      status: 404\n    - url: https://www.apptio.com/.well-known/oauth-authorization-server\n      status: 404\n  note: >-\n    End-user SSO into the Apptio Frontdoor console is SAML-based\n    (frontdoor.apptio.com issues a SAMLRequest to the customer IdP, observed live\n    on 2026-09-05 when api.apptio.com 303s to the login flow). That is console\n    sign-in, not API authorization, and grants no API token by\
  \ itself.\nhosts:\n  - region: Americas (US)\n    host: api.cloudability.com\n    api_key: true\n    opentoken: true\n  - region: US Government Cloud\n    host: api.usgov.cloudability.com\n    api_key: false\n    opentoken: true\n  - region: Australia / APAC\n    host: api-au.cloudability.com\n    api_key: true\n    opentoken: true\n  - region: Europe\n    host: api-eu.cloudability.com\n    api_key: true\n    opentoken: true\n  - region: Middle East\n    host: api-me.cloudability.com\n    api_key: true\n    opentoken: true\n  - region: Canada\n    host: api-ca.cloudability.com\n    api_key: true\n    opentoken: true\n  - region: India\n    host: api-in.cloudability.com\n    api_key: true\n    opentoken: true\n  - region: Japan\n    host: api-jp.cloudability.com\n    api_key: true\n    opentoken: true\n  - region: Singapore\n    host: api-sg.cloudability.com\n    api_key: true\n    opentoken: true\nunauthenticated_response:\n  probed: '2026-09-05'\n  url: https://api.cloudability.com/v3\n\
  \  status: 401\n  content_type: application/json\n  www_authenticate: absent\n  body: >-\n    {\"error\":{\"status\":401,\"code\":\"unauthorized\",\"messages\":[\"missing auth\n    tokens\"],\"uniqueid\":\"...\",\"typeid\":\"...\",\"traceid\":\"...\"}}\n  note: >-\n    The 401 is returned for EVERY path on the host, including paths that do not\n    exist (control probe /zzz-does-not-exist-9482 -> 401). No WWW-Authenticate\n    challenge is emitted, so a client cannot discover the scheme from the\n    response — it has to read the documentation.\npermissions:\n  model: feature-permission\n  note: >-\n    Endpoints are gated by named Cloudability feature permissions rather than\n    OAuth scopes — for example the v3 Users endpoints require\n    \"UserManagementFeatureFullAccess\". IBM does not publish a consolidated\n    permission reference, so no scopes artifact is written.\ndocumentation_inconsistency:\n  observed: '2026-09-05'\n  note: >-\n    IBM's own v3 reference does not describe\
  \ one credential consistently. The\n    getting-started page documents `Authorization: Basic <cldy_token>`, while the\n    Views end point page states that every Views operation requires \"a valid bearer\n    token\" in the Authorization header. No page reconciles the two, and there is no\n    OpenAPI securityScheme to settle it, so a client integrating against the Views\n    endpoints cannot tell from the documentation whether to send Basic or Bearer.\n  evidence:\n    - url: https://www.ibm.com/docs/en/cloudability-commercial/cloudability-premium/saas?topic=api-getting-started-cloudability-v3\n      says: 'Authorization: Basic <cldy_token>'\n    - url: https://www.ibm.com/docs/en/cloudability-commercial/cloudability-premium/saas?topic=api-views-end-point\n      says: '\"a valid bearer token\" in the Authorization header'\n  wire_evidence: >-\n    The live 401 from https://api.cloudability.com/v3 emits no WWW-Authenticate\n    header, so the ambiguity cannot be resolved by observation\
  \ either.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudability/refs/heads/main/authentication/cloudability-authentication.yml
summary_line: 2 schemes
tags:
- Cloud Cost Management
- Cost Optimization
- FinOps
- Multi-Cloud
- Recommendations
- Reporting
---
