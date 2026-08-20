---
api_key_in: []
api_specs:
- filename: tsinghua-mirror-status-api-openapi.yml
  format: yaml
  label: Tsinghua University TUNA Open Source Mirror
  slug: tsinghua-mirror-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsinghua/refs/heads/main/openapi/tsinghua-mirror-status-api-openapi.yml
- filename: tsinghua-identity-federation-api-openapi.yml
  format: yaml
  label: Tsinghua University Identity Provider — SAML 2.0 Federation Metadata
  slug: identity-federation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tsinghua/refs/heads/main/openapi/tsinghua-identity-federation-api-openapi.yml
auth_types: []
description: 'How access is established across Tsinghua University''s surfaces. There are only two regimes, and the split between them is the whole story of this profile: everything the university itself runs for its own staff and students sits behind one campus identity service, and the only unauthenticated machine-readable endpoints belong to the student-run TUNA open-source mirror. No developer portal, no API key issuance, no OAuth client registration and no self-service credentialing of any kind was found on a Tsinghua host.'
kind: authentication
layout: security
method: probed
name: Tsinghua Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tsinghua University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Tsinghua University
provider_slug: tsinghua
scheme_count: 0
schemes: []
slug: tsinghua-authentication
source_filename: tsinghua-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Tsinghua University — authentication\ndescription: >-\n  How access is established across Tsinghua University's surfaces. There are only two regimes,\n  and the split between them is the whole story of this profile: everything the university itself\n  runs for its own staff and students sits behind one campus identity service, and the only\n  unauthenticated machine-readable endpoints belong to the student-run TUNA open-source mirror.\n  No developer portal, no API key issuance, no OAuth client registration and no self-service\n  credentialing of any kind was found on a Tsinghua host.\ngenerated: '2026-08-19'\nmodified: '2026-08-19'\nmethod: probed\nsource: >-\n  Live HTTP probes of tsinghua.edu.cn hosts on 2026-08-19, plus the SAML 2.0 metadata Tsinghua\n  publishes at https://idp.tsinghua.edu.cn/idp/shibboleth.\nx-operator: institution\nmechanisms:\n  - id: anonymous-public\n    name: Open / no credential\n    type: none\n    method: probed\n    source: live 200 responses,\
  \ 2026-08-19\n    applies_to:\n      - Tsinghua University TUNA Mirror Status API\n      - Tsinghua University TUNA Mirror ISO Image Catalog API\n      - Tsinghua University Identity Provider — SAML 2.0 federation metadata\n    evidence:\n      - url: https://mirrors.tuna.tsinghua.edu.cn/static/tunasync.json\n        status: 200\n      - url: https://mirrors.tuna.tsinghua.edu.cn/static/status/isoinfo.json\n        status: 200\n      - url: https://idp.tsinghua.edu.cn/idp/shibboleth\n        status: 200\n    note: >-\n      These three answer an anonymous client with no header of any kind. They are the entire\n      unauthenticated machine-readable footprint found for this institution.\n  - id: edge-user-agent-filter\n    name: User-Agent filtering at the mirror edge\n    type: none\n    method: probed\n    source: live probes, 2026-08-19\n    applies_to:\n      - Tsinghua University TUNA Mirror Status API\n      - Tsinghua University TUNA Mirror ISO Image Catalog API\n    evidence:\n \
  \     - url: https://mirrors.tuna.tsinghua.edu.cn/static/tunasync.json\n        status: 403\n        note: 'User-Agent: Mozilla/5.0 … Chrome/126.0 Safari/537.36 — HTML \"access denied\" page, 15,345 bytes'\n      - url: https://mirrors.tuna.tsinghua.edu.cn/static/tunasync.json\n        status: 200\n        note: 'User-Agent: curl/8.7.1 — application/json, 74,172 bytes'\n    note: >-\n      Not an authentication mechanism, recorded here because it behaves like one for any client\n      that guesses wrong. The mirror edge answers 403 with a trilingual HTML denial page to\n      requests carrying a desktop-browser User-Agent while answering the identical request with\n      a plain tool User-Agent 200. This is the inverse of the usual bot filter and it means a\n      naive agent that spoofs a browser is locked out of the one open API this institution has.\n  - id: campus-sso\n    name: Tsinghua electronic identity service (id.tsinghua.edu.cn) — OAuth-style redirect + SAML/Shibboleth\n   \
  \ type: sso\n    method: probed\n    source: live redirect chains, 2026-08-19\n    applies_to:\n      - Tsinghua Cloud (cloud.tsinghua.edu.cn)\n      - Tsinghua GitLab (git.tsinghua.edu.cn)\n      - Tsinghua Web Learning / 网络学堂 (learn.tsinghua.edu.cn)\n      - Tsinghua course registration (zhjwxk.cic.tsinghua.edu.cn)\n      - Information portal (info.tsinghua.edu.cn), campus card (card.tsinghua.edu.cn)\n    evidence:\n      - url: https://cloud.tsinghua.edu.cn/\n        status: 200\n        note: redirects to id.tsinghua.edu.cn/do/off/ui/auth/login/form/… with a /thu-oauth/callback return target\n      - url: https://git.tsinghua.edu.cn/\n        status: 200\n        note: GitLab sign-in page whose only form posts to /users/auth/thuid\n      - url: https://learn.tsinghua.edu.cn/\n        status: 200\n        note: redirects to /f/login (清华大学网络学堂 login)\n      - url: https://zhjwxk.cic.tsinghua.edu.cn/\n        status: 200\n        note: redirects to the same id.tsinghua.edu.cn login form\n\
  \      - url: https://idp.tsinghua.edu.cn/idp/shibboleth\n        status: 200\n        note: SAML 2.0 / Shibboleth metadata for the federation side of the same identity estate\n    note: >-\n      Every institution-run system found in this pass terminates at id.tsinghua.edu.cn. The\n      redirect carries an OAuth-shaped callback (/thu-oauth/callback) and the federation side is\n      Shibboleth SAML 2.0, but neither publishes a client-registration path, a scope list, a\n      discovery document or an authorization-server metadata endpoint that an outside developer\n      could use. Access is granted by institutional affiliation, not by credentialing.\nno_public_credentialing:\n  checked: '2026-08-19'\n  detail: >-\n    No API key signup, no OAuth client registration, no developer terms and no rate-limit or quota\n    documentation was found on any Tsinghua host. api.tsinghua.edu.cn, open.tsinghua.edu.cn and\n    data.tsinghua.edu.cn do not resolve.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tsinghua/refs/heads/main/authentication/tsinghua-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- China
- Beijing
- C9 League
- Research
- Open-Source
- Mirror
- Identity Federation
- Shibboleth
- SAML
- Research Data
- DOI
- Library
---
