---
api_key_in:
- header
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Centrical Authentication
name_suffix: Authentication
oauth_flows: []
overview: Centrical declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Centrical
provider_slug: centrical
scheme_count: 0
schemes: []
slug: centrical-authentication
source_filename: centrical-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: Access-Control-Allow-Headers served by app.centrical.me, docs.centrical.me and powerup.centrical.me\npublished_by_provider: false\n\n# READ THIS BEFORE USING THIS FILE.\n#\n# Centrical publishes NO authentication documentation. There is no developer portal, no auth page,\n# no OpenAPI securitySchemes, and no OIDC/OAuth discovery document — /.well-known/openid-configuration\n# and /.well-known/oauth-authorization-server both 404 on centrical.com and 403 on api.centrical.me.\n#\n# Everything below is INFERRED from one thing Centrical's own edge emits anonymously: the\n# Access-Control-Allow-Headers list its application hosts return on every response. That header\n# enumerates the request headers the platform is willing to accept, which names the credential\n# headers by name. That is real, observed, reproducible evidence of the auth surface's SHAPE — it is\n# not a contract, it does not tell us how to obtain a credential, and it\
  \ must never be presented as\n# Centrical-published documentation.\n#\n# For this reason NO `type: Authentication` pointer is wired into apis.yml. The\n# `authentication_documented` check asks whether the PROVIDER documents authentication. Centrical\n# does not. This file records what we could see, and names the gap.\n\nnote: >-\n  Inferred auth surface only. Centrical documents authentication to contracted customers inside its\n  Zendesk help center (401 anonymously). No pointer is emitted; this artifact is evidence, not a\n  published contract.\n\nsummary:\n  types_inferred: [apiKey, http-bearer-jwt, sso-token]\n  api_key_in: [header]\n  oauth2_flows: []\n  oidc_discovery: false\n  documented: false\n\ninferred_schemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  confidence: high\n  evidence: >-\n    `x-api-key` is listed in Access-Control-Allow-Headers on every Centrical application host. It is\n    also the canonical AWS API Gateway key header,\
  \ and api.centrical.me is an AWS API Gateway custom\n    domain (x-amzn-errortype: ForbiddenException), which is consistent with key-based edge auth.\n- name: jwt\n  type: apiKey\n  in: header\n  parameter_name: jwt\n  confidence: medium\n  evidence: >-\n    A bare `jwt` request header is accepted alongside the standard `authorization` header. Which of\n    the two carries the bearer token for the integration API is not determinable anonymously.\n- name: authorization\n  type: http\n  scheme: bearer\n  confidence: medium\n  evidence: Standard `authorization` header is in the accepted list.\n- name: ssoToken\n  type: apiKey\n  in: header\n  parameter_name: ssoToken\n  confidence: medium\n  evidence: >-\n    `ssoToken` is accepted, and powerup.centrical.me returns an `ssoredirect` response header —\n    consistent with the enterprise SSO Centrical markets to customers. No SAML/OIDC metadata endpoint\n    is public.\n- name: Signature\n  type: apiKey\n  in: header\n  parameter_name: Signature\n\
  \  confidence: low\n  evidence: >-\n    A `Signature` header is accepted, suggesting request signing on some surface (possibly webhook or\n    inbound callback verification). No algorithm, canonicalization or key distribution is documented.\n\n# Non-credential headers the same CORS policy advertises. Captured here rather than in a\n# conventions/ artifact because Centrical documents none of them — there is no conventions contract\n# to record, only observed header names.\nobserved_platform_headers:\n- {header: centri-version, inferred_purpose: API/platform version selection, confidence: medium}\n- {header: centri-request-id, inferred_purpose: request correlation / tracing id, confidence: medium}\n- {header: session-id, inferred_purpose: session correlation, confidence: medium}\n- {header: 'x-cen-1', inferred_purpose: unknown vendor header, confidence: low}\n- {header: 'g-s-x', inferred_purpose: unknown legacy GamEffective header, confidence: low}\n- {header: 'g-s-x-t', inferred_purpose:\
  \ unknown legacy GamEffective header, confidence: low}\n- {header: 'g-s-i-i', inferred_purpose: unknown legacy GamEffective header, confidence: low}\n- {header: fromMobile, inferred_purpose: client-surface flag, confidence: low}\n- {header: fromAdmin, inferred_purpose: client-surface flag, confidence: low}\n- {header: fromGameapp, inferred_purpose: client-surface flag, confidence: low}\n- {header: fromGtv, inferred_purpose: client-surface flag, confidence: low}\n- {header: ManagerOrgUnitId, inferred_purpose: org-unit scoping / impersonation context, confidence: low}\n- {header: ManagerOrgUnitUserName, inferred_purpose: org-unit scoping / impersonation context, confidence: low}\n- {header: LoggedBy, inferred_purpose: actor attribution, confidence: low}\n- {header: 'GE-IGNORE-CACHE', inferred_purpose: cache bypass (GE = GamEffective), confidence: low}\n- {header: game-id, inferred_purpose: game/program scoping, confidence: low}\n\nraw_cors_allow_headers: >-\n  accept, authorization, content-type,\
  \ Cache-Control, P3P, GE-IGNORE-CACHE, Signature, fromMobile,\n  ssoToken, fromAdmin, fromGameapp, fromGtv, ManagerOrgUnitUserName, ManagerOrgUnitId, g-s-x,\n  g-s-x-t, g-s-i-i, User-Agent, Referer, Origin, Access-Control-Allow-Headers, x-cen-1, jwt,\n  x-api-key, centri-request-id, session-id, centri-version, LoggedBy, test-name, game-id\n\nallowed_methods: [GET, POST, PUT, OPTIONS, HEAD]\n\ngap_to_close_upstream: >-\n  Centrical could make this an actual artifact by publishing one anonymous page describing how an\n  integrator obtains a credential and which header carries it. Today the only public signal that any\n  of this exists is a CORS preflight allowlist.\n\nx-evidence:\n- {url: 'https://app.centrical.me/', status: 302, checked: '2026-08-10', note: Access-Control-Allow-Headers observed}\n- {url: 'https://docs.centrical.me/', status: 302, checked: '2026-08-10', note: Access-Control-Allow-Headers observed}\n- {url: 'https://powerup.centrical.me/', status: 302, checked: '2026-08-10',\
  \ note: ssoredirect header observed}\n- {url: 'https://api.centrical.me/.well-known/openid-configuration', status: 403, checked: '2026-08-10'}\n- {url: 'https://api.centrical.me/.well-known/oauth-authorization-server', status: 403, checked: '2026-08-10'}\n- {url: 'https://centrical.com/.well-known/openid-configuration', status: 404, checked: '2026-08-09'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centrical/refs/heads/main/authentication/centrical-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Employee Engagement
- Performance Management
- Gamification
- Microlearning
- Contact Center
- Workforce Engagement Management
- Coaching
- Quality Management
- Human Resources
- Software-as-a-Service
---
