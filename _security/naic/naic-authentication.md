---
api_key_in: []
api_specs:
- filename: naic-content-jsonapi-openapi.yml
  format: yaml
  label: NAIC Content JSON:API
  slug: content-jsonapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/naic/refs/heads/main/openapi/naic-content-jsonapi-openapi.yml
auth_types:
- none
- cookie
- saml-oidc-sso
description: ''
kind: authentication
layout: security
method: searched
name: Naic Authentication
name_suffix: Authentication
oauth_flows: []
overview: NAIC secures its APIs with none, cookie, and saml-oidc-sso across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NAIC
provider_slug: naic
scheme_count: 0
schemes: []
slug: naic-authentication
source_filename: naic-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  Live probes of content.naic.org, api.naic.org, eapps.naic.org, sbs.naic.org,\n  services.serff.com and services-beta.serff.com on 2026-07-25, plus the SERFF Technical\n  Support Checklist at serff.com.\ndocs: null\ndocs_note: >-\n  The NAIC publishes no authentication documentation for any machine surface. This profile was\n  established entirely by probing. derive-authentication.py was not used because the only\n  OpenAPI in this repo is one API Evangelist derived from the live JSON:API index, and it\n  declares no securitySchemes — the read surface genuinely has none.\n\nsummary:\n  types: [none, cookie, saml-oidc-sso]\n  api_key_in: []\n  oauth2_flows: []\n  public_read_without_credentials: true\n  self_serve_signup: false\n  oauth_metadata_published: false\n\nsurfaces:\n\n- name: NAIC Content JSON:API\n  host: https://content.naic.org/jsonapi\n  audience: public\n  scheme: none\n  read: anonymous\n  evidence: >-\n\
  \    Anonymous GET returned HTTP 200 application/vnd.api+json on every content collection\n    probed (node--article, node--page, node--committee_page, node--state_department_contact,\n    taxonomy_term--model_laws, taxonomy_term--states, taxonomy_term--insurance_types,\n    taxonomy_term--publications, media--document, node--newsletter, user--user). No API key,\n    bearer token, cookie or referer was sent.\n  write: closed\n  write_evidence: >-\n    POST /jsonapi/node/article returned HTTP 401 with detail \"No authentication credentials\n    provided.\"; DELETE returned HTTP 405 with \"Allow: GET, HEAD, POST\".\n  credentialing_path: >-\n    None published. Drupal would authenticate writes with a session cookie or, if enabled, HTTP\n    Basic / OAuth — but no signup, no key issuance and no documentation exist, so the write\n    surface is effectively unreachable for third parties.\n  caveat: >-\n    Because reads are anonymous, there is also no per-caller identity, no quota and no\n\
  \    revocation. Consumption etiquette is the only control: see the crawl_delay and\n    max_requests_per_day the NAIC publishes in llms/naic-llms.txt.\n\n- name: NAIC regulator and industry portals (myNAIC, iSite+, SBS, OPTins, InsData, SERFF Login)\n  hosts:\n  - https://eapps.naic.org/\n  - https://isiteplus.naic.org/\n  - https://sbs.naic.org/\n  - https://insdata.naic.org/\n  audience: partner-only\n  scheme: Okta-fronted SSO (SAML / OIDC), interactive browser login\n  evidence: >-\n    eapps.naic.org returns HTTP 200 for both /.well-known/openid-configuration and\n    /.well-known/oauth-authorization-server, but with `content-type: text/html;charset=utf-8`\n    rendering the Okta Sign-In Widget 7.35.3 — a catch-all login route, NOT an OIDC discovery\n    document. No anonymous OAuth/OIDC metadata is served anywhere on the estate. Re-verified\n    2026-07-25.\n  self_serve: false\n  note: >-\n    These are human web applications behind SSO, not delegated-authorization API surfaces.\
  \ No\n    OAuth client registration, no scopes, no token endpoint is exposed to third parties, which\n    is why scopes/ is deliberately absent from this repo.\n\n- name: SERFF Web Services (Legacy SPI, Legacy SIS, Modernized Data API)\n  hosts:\n  - https://services.serff.com/\n  - https://services-beta.serff.com/\n  audience: partner-only\n  scheme: per-integrator credentials issued by the NAIC on request\n  provisioning: email wsrequest@naic.org\n  evidence: >-\n    services.serff.com returns HTTP 403 anonymously at the root. The SERFF Technical Support\n    Checklist names the three services and their PROD/BETA environments but publishes no auth\n    scheme, no endpoint list, no WSDL and no OpenAPI.\n  self_serve: false\n\n- name: api.naic.org\n  host: https://api.naic.org/\n  audience: internal\n  scheme: unknown\n  evidence: >-\n    Host resolves and answers over HTTP/2 but returns a bare `text/plain` 404 \"Not Found\" on /,\n    /openapi.json, /openapi.yaml, /swagger.json, /v1/openapi.json,\
  \ /api-docs, /docs, /redoc,\n    /graphql, /.well-known/openid-configuration and /.well-known/oauth-authorization-server\n    (re-probed 2026-07-25). An internal gateway with no public surface and no advertised auth.\n\nwell_known:\n  oauth_authorization_server: not published\n  oauth_protected_resource: not published\n  openid_configuration: not published\n  detail: >-\n    See well-known/naic-well-known.yml. The only two hosts that answer 200 on a /.well-known/\n    OAuth path (eapps.naic.org) serve an HTML login page, not metadata — recorded as a\n    false-positive trap rather than as discovery documents.\n\ncross_links:\n  conventions: conventions/naic-conventions.yml\n  errors: errors/naic-problem-types.yml\n  well_known: well-known/naic-well-known.yml\n  domain_security: security/naic-domain-security.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/naic/refs/heads/main/authentication/naic-authentication.yml
summary_line: none/cookie/saml-oidc-sso · 0 schemes
tags:
- Insurance
- United States
- Regulator
- Market Infrastructure
- Insurance Regulation
- Property and Casualty
- Life Insurance
- Health Insurance
- Producer Licensing
- Rate and Form Filing
- Regulatory Reporting
- Standards Body
- Model Laws
- Regulatory Data
- Open Data
---
