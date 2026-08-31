---
api_key_in: []
auth_types: []
description: How each machine-readable surface attributed to the University of Otago authenticates, as observed from live probes rather than from documentation. Every status code below was returned to an unauthenticated request from a public network on 2026-08-30.
kind: authentication
layout: security
method: probed
name: University Of Otago Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Otago declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Otago
provider_slug: university-of-otago
scheme_count: 0
schemes: []
slug: university-of-otago-authentication
source_filename: university-of-otago-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: University of Otago — Authentication Posture\ndescription: >-\n  How each machine-readable surface attributed to the University of Otago authenticates, as\n  observed from live probes rather than from documentation. Every status code below was returned\n  to an unauthenticated request from a public network on 2026-08-30.\nurl: https://raw.githubusercontent.com/api-evangelist/university-of-otago/refs/heads/main/authentication/university-of-otago-authentication.yml\ncreated: '2026-08-30'\nmodified: '2026-08-30'\ngenerated: '2026-08-30'\nmethod: probed\nsource: Unauthenticated HTTP probes executed 2026-08-30 with a browser User-Agent.\n\nsurfaces:\n  - aid: university-of-otago:ai-site-wp-rest\n    x-operator: institution\n    scheme: none\n    public_read: true\n    detail: >-\n      The WordPress REST API at artificialintelligence.otago.ac.nz declares an empty\n      \"authentication\": [] object in its discovery document and serves published content to\n      anonymous\
  \ callers: /wp-json/ returns the full 144-route index (200) and\n      /wp-json/wp/v2/pages returns page objects (200) with no credential. Write methods\n      (POST/PUT/PATCH/DELETE) are advertised in the route table but require a WordPress\n      session or application password that is not publicly issued. This is the only surface in\n      this repo that answers with institution-owned data and no credential.\n    evidence:\n      - url: https://artificialintelligence.otago.ac.nz/wp-json/\n        status: 200\n      - url: https://artificialintelligence.otago.ac.nz/wp-json/wp/v2/pages\n        status: 200\n\n  - aid: university-of-otago:our-archive-oai\n    x-operator: tenant\n    scheme: gated\n    public_read: false\n    detail: >-\n      OAI-PMH harvesting is deployed but not authorised for the public. Every verb returns\n      HTTP 403 with OAI error_code 21, \"Unauthorized access to the OAI services\". There is no\n      documented public path to obtain authorisation; Ex Libris\
  \ Esploro gates OAI at the tenant\n      configuration level, so enabling it is Otago's decision and Ex Libris's switch. The\n      repository's human interface and its sitemap index are open.\n    evidence:\n      - url: https://ourarchive.otago.ac.nz/view/oai/64OTAGO_INST/request?verb=Identify\n        status: 403\n      - url: https://ourarchive.otago.ac.nz/view/google/siteindex.xml\n        status: 200\n      - url: https://ourarchive.otago.ac.nz/esploro/?institution=64OTAGO_INST\n        status: 200\n\n  - aid: university-of-otago:blackboard-learn\n    x-operator: tenant\n    scheme: oauth2\n    public_read: partial\n    detail: >-\n      Blackboard Learn's REST API is deployed and reachable. One endpoint answers keyless —\n      /learn/api/public/v1/system/version returns {\"learn\":{\"major\":4000,\"minor\":21,\"patch\":0,\n      \"build\":\"rel.28+435d029\"}} (200). Every data endpoint returns HTTP 401 with the JSON body\n      {\"status\":401,\"message\":\"API request is not authenticated.\"\
  } — /learn/api/public/v1/courses,\n      /learn/api/public/v1/dataSources and /learn/api/public/v3/courses were all confirmed. A 401\n      rather than a 404 is the evidence that the API exists and is gated. Credentials are\n      REST application keys issued only by Otago administrators through the Anthology developer\n      portal; there is no self-service signup.\n    evidence:\n      - url: https://blackboard.otago.ac.nz/learn/api/public/v1/system/version\n        status: 200\n      - url: https://blackboard.otago.ac.nz/learn/api/public/v1/courses\n        status: 401\n      - url: https://blackboard.otago.ac.nz/learn/api/public/v1/dataSources\n        status: 401\n      - url: https://blackboard.otago.ac.nz/learn/api/public/v3/courses\n        status: 401\n\n  - aid: university-of-otago:tuakiri-idp\n    x-operator: tenant\n    scheme: saml2\n    public_read: metadata_only\n    detail: >-\n      Browser-mediated SAML 2.0 web SSO. There is no bearer token, API key or client-credentials\n\
  \      path: an integration becomes a Tuakiri service provider and receives assertions, it does\n      not call an endpoint. The federation METADATA is fully public and machine-readable from the\n      signed aggregate (200). The SSO endpoint itself is not meaningfully callable outside a SAML\n      flow — a bare GET to the Redirect/SSO binding returns HTTP 500, which is the expected\n      response to a request carrying no AuthnRequest, not a fault in the service.\n    evidence:\n      - url: https://directory.tuakiri.ac.nz/metadata/tuakiri-metadata-signed.xml\n        status: 200\n      - url: https://hosted-login.tuakiri.ac.nz/hosting/otago.ac.nz/idp/profile/SAML2/Redirect/SSO\n        status: 500\n\n  - aid: university-of-otago:scholarly-identifiers\n    x-operator: tenant\n    scheme: none\n    public_read: true\n    detail: >-\n      Otago's DataCite and Crossref registrations are readable without credentials through each\n      registry's own public REST API. Otago authenticates\
  \ to DEPOSIT (DataCite repository\n      accounts otagouni.snbodh / otagouni.qmyzok, Crossref member 4843 depositor credentials);\n      the public may READ the resulting records anonymously. The credentials belong to Otago;\n      the endpoints belong to the registries.\n    evidence:\n      - url: https://api.datacite.org/providers/otagouni\n        status: 200\n      - url: https://api.crossref.org/members/4843\n        status: 200\n\nnot_authenticable:\n  - url: https://api.otago.ac.nz/\n    status: 503\n    detail: >-\n      Institution-owned hostname behind Cloudflare, but the origin is an OpenShift router\n      returning the default \"Application is not available\" page on every path probed\n      (/, /openapi.json, /swagger, /docs, /api, /v1, /health, /.well-known/openapi). There is\n      nothing to authenticate against. Not recorded as a surface.\n  - url: https://login.otago.ac.nz/\n    status: 0\n    detail: >-\n      Resolves to a campus address (139.80.64.89 via its-cs-im.registry.otago.ac.nz)\
  \ but does\n      not complete a connection from a public network. A real internal identity service that is\n      not publicly callable, and is not credited as a surface.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-otago/refs/heads/main/authentication/university-of-otago-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- New Zealand
- Research
- Research Repository
- Open Access
- Repository
- Identity Federation
- Shibboleth
- SAML
- OAI-PMH
- Learning Management
- DataCite
- Crossref
- Metadata
- Library
---
