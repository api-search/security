---
api_key_in: []
api_specs:
- filename: keio-koara-oai-pmh-openapi.yml
  format: yaml
  label: KOARA OAI-PMH Metadata API
  slug: koara-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keio/refs/heads/main/openapi/keio-koara-oai-pmh-openapi.yml
- filename: keio-iiif-openapi.yml
  format: yaml
  label: Keio Media Center Digital Collections IIIF API
  slug: iiif
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keio/refs/heads/main/openapi/keio-iiif-openapi.yml
auth_types: []
description: 'Keio University''s authentication posture splits cleanly in two, and the split is the most useful thing to say about it. The surfaces the university operates itself for the public — the KOARA OAI-PMH interface and the Media Center''s IIIF endpoints — require no authentication of any kind: no key, no token, no registration, no referer check, no rate-limit header. The surfaces that serve the campus — the K-RIS research information system, the K-LMS learning environment, and every application behind gslbs.keio.jp — are gated behind federated institutional identity, and there is no path by which an unaffiliated developer obtains a credential. There is no developer portal, no key-issuance form and no client-registration endpoint an outsider can use anywhere in the estate.'
kind: authentication
layout: security
method: derived
name: Keio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keio University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Keio University
provider_slug: keio
scheme_count: 0
schemes: []
slug: keio-authentication
source_filename: keio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: derived\nauthorship: API Evangelist\nprobe_basis: live probe sweep of Keio University surfaces, 2026-09-01\nsource: >-\n  Live anonymous probes of every Keio surface named in apis.yml on 2026-09-01. Each authentication\n  claim below is the observed behaviour of a real request, not a reading of documentation — Keio\n  publishes no developer authentication documentation for any of these surfaces.\nprovider: Keio University\nproviderId: keio\ndescription: >-\n  Keio University's authentication posture splits cleanly in two, and the split is the most useful\n  thing to say about it. The surfaces the university operates itself for the public — the KOARA\n  OAI-PMH interface and the Media Center's IIIF endpoints — require no authentication of any kind:\n  no key, no token, no registration, no referer check, no rate-limit header. The surfaces that\n  serve the campus — the K-RIS research information system, the K-LMS learning environment, and\n  every\
  \ application behind gslbs.keio.jp — are gated behind federated institutional identity, and\n  there is no path by which an unaffiliated developer obtains a credential. There is no developer\n  portal, no key-issuance form and no client-registration endpoint an outsider can use anywhere in\n  the estate.\n\nsurfaces:\n  - name: KOARA OAI-PMH Metadata API\n    baseURL: https://koara.lib.keio.ac.jp/xoonips/modules/xoonips/oai.php\n    x-operator: institution\n    scheme: none\n    detail: >-\n      Anonymous. A bare GET with a verb returns a complete OAI-PMH response. No Authorization\n      header, cookie, key or referer is required or honoured. robots.txt at the host is\n      `User-agent: * / Allow: /`.\n    probed_status: 200\n\n  - name: Keio Media Center IIIF Presentation and Image APIs\n    baseURL: https://dcollections.lib.keio.ac.jp/sites/default/files/iiif/\n    x-operator: institution\n    scheme: none\n    detail: >-\n      Anonymous. Manifests and image tiles are served without\
  \ authentication or a IIIF Authentication\n      API service block. No `service` of `@type: AuthCookieService1` appears in the manifest, so\n      there is no degraded-access or login-required tier — the collections are open.\n    probed_status: 200\n\n  - name: Keio Okta tenant (keio.okta.com)\n    baseURL: https://keio.okta.com\n    x-operator: tenant\n    scheme: oauth2 / oidc\n    detail: >-\n      OpenID Connect discovery is anonymously readable at\n      https://keio.okta.com/.well-known/openid-configuration and advertises authorization, token,\n      userinfo, jwks and a dynamic client registration endpoint. In practice a client_id exists only\n      if Keio IT creates one; the registration endpoint is Okta's standard org endpoint and is not\n      open to unaffiliated callers. Readable, not consumable.\n    probed_status: 200\n    flows_advertised:\n      - code\n      - id_token\n      - code id_token\n      - code token\n      - id_token token\n      - code id_token token\n\n\
  \  - name: GakuNin / eduGAIN SAML identity provider\n    entityID: https://gakunin1.keio.ac.jp/idp/shibboleth\n    x-operator: institution\n    scheme: saml2\n    detail: >-\n      SAML 2.0 web browser SSO, transient NameID only. Access is granted to service providers\n      registered in GakuNin or reachable through eduGAIN, not to individual developers. Requires an\n      institutional or federation relationship, never an API key.\n    probed_status: 200\n\n  - name: K-RIS (Keio Research Information System)\n    baseURL: https://k-ris.keio.ac.jp/\n    x-operator: tenant\n    scheme: session\n    detail: >-\n      The public researcher-profile portal renders anonymously, but the Pure web service path\n      (/ws/api and /ws/api/openapi.json) returns 404 — the machine-readable interface is not exposed\n      on this deployment. No API credential is obtainable.\n    probed_status: 404\n\nnot_found:\n  - what: Developer portal or API key issuance\n    detail: >-\n      No api.keio.ac.jp\
  \ (NXDOMAIN), no data.keio.ac.jp (NXDOMAIN), no developer portal, no key\n      request form, and no API terms document anywhere on the estate.\n  - what: security.txt\n    detail: https://www.keio.ac.jp/.well-known/security.txt returns a real HTTP 404.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keio/refs/heads/main/authentication/keio-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Japan
- Research
- Institutional Repository
- Research Repository
- Identity Federation
- Digital Collections
- IIIF
- OAI-PMH
- Open Access
- Cultural Heritage
---
