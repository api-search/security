---
api_key_in: []
api_specs:
- filename: universiti-teknologi-petronas-utpedia-openapi.yml
  format: yaml
  label: UTPedia Institutional Repository
  slug: utpedia
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/universiti-teknologi-petronas/refs/heads/main/openapi/universiti-teknologi-petronas-utpedia-openapi.yml
- filename: universiti-teknologi-petronas-scholars-openapi.yml
  format: yaml
  label: UTP Scholarly Publication Repository
  slug: scholars
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/universiti-teknologi-petronas/refs/heads/main/openapi/universiti-teknologi-petronas-scholars-openapi.yml
auth_types: []
description: How each machine-readable surface Universiti Teknologi PETRONAS operates or holds a tenancy in handles authentication, established by probing each endpoint without credentials on 2026-09-01. No credential was supplied, guessed, or obtained at any point.
kind: authentication
layout: security
method: probed
name: Universiti Teknologi Petronas Authentication
name_suffix: Authentication
oauth_flows: []
overview: Universiti Teknologi PETRONAS declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Universiti Teknologi PETRONAS
provider_slug: universiti-teknologi-petronas
scheme_count: 0
schemes: []
slug: universiti-teknologi-petronas-authentication
source_filename: universiti-teknologi-petronas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: Universiti Teknologi PETRONAS — authentication posture\ndescription: >-\n  How each machine-readable surface Universiti Teknologi PETRONAS operates or holds a tenancy in\n  handles authentication, established by probing each endpoint without credentials on 2026-09-01.\n  No credential was supplied, guessed, or obtained at any point.\ngenerated: '2026-09-01'\nmodified: '2026-09-01'\nmethod: probed\nsource: unauthenticated HTTP probes, 2026-09-01\nsurfaces:\n  - surface: UTPedia OAI-PMH\n    url: https://utpedia.utp.edu.my/cgi/oai2\n    x-operator: institution\n    auth: none\n    observed_status: 200\n    detail: Fully open metadata harvesting. No key, no registration, no rate-limit header observed.\n  - surface: UTPedia EPrints REST (read)\n    url: https://utpedia.utp.edu.my/rest/\n    x-operator: institution\n    auth: none\n    observed_status: 200\n    detail: >-\n      Datasets eprint, subject and user all return 200 unauthenticated. Record retrieval at\n  \
  \    /rest/eprint/{id}.xml is open; an unknown id returns 404.\n  - surface: UTPedia JSON export\n    url: https://utpedia.utp.edu.my/cgi/export/eprint/376/JSON/utpedia-eprint-376.js\n    x-operator: institution\n    auth: none\n    observed_status: 200\n    detail: application/json served without authentication for this record.\n  - surface: UTP Scholarly Publication JSON export\n    url: https://scholars.utp.edu.my/cgi/export/eprint/205/JSON/scholars-eprint-205.js\n    x-operator: institution\n    auth: basic\n    observed_status: 401\n    detail: >-\n      The sibling repository gates its JSON export behind HTTP Basic where UTPedia does not — the\n      two EPrints deployments are configured differently. OAI-PMH and REST read on this host\n      remain open.\n  - surface: SWORD deposit service document (both repositories)\n    url: https://utpedia.utp.edu.my/sword-app/servicedocument\n    x-operator: institution\n    auth: basic\n    observed_status: 401\n    detail: Deposit is credentialed.\
  \ Present but not usable by the public; no attempt was made.\n  - surface: Moodle web services (uLearn)\n    url: https://ulearn.utp.edu.my/webservice/rest/server.php\n    x-operator: tenant\n    auth: token\n    observed_status: 200\n    detail: >-\n      Returns a structured Moodle exception — ERRORCODE invalidtoken, \"Invalid token - token not\n      found\" — so the web-service layer is enabled and expects a wstoken. Tokens are issued to\n      enrolled users, not to the public.\n  - surface: LTI 1.3 platform keys (uLearn)\n    url: https://ulearn.utp.edu.my/mod/lti/certs.php\n    x-operator: tenant\n    auth: none\n    observed_status: 200\n    detail: Public JWKS, as LTI 1.3 requires. RS256.\n  - surface: Microsoft Entra ID tenant (utp.edu.my)\n    url: https://login.microsoftonline.com/utp.edu.my/v2.0/.well-known/openid-configuration\n    x-operator: federation\n    auth: oauth2\n    observed_status: 200\n    detail: >-\n      OIDC discovery and SAML 2.0 federation metadata are\
  \ public by design; the endpoints they\n      describe are the institution's own single-sign-on, tenant\n      84187be3-037e-41ec-889c-a150fe476432.\n  - surface: UCS single sign-on\n    url: https://ucs.utp.edu.my/SignIn\n    x-operator: institution\n    auth: interactive\n    observed_status: 200\n    detail: >-\n      Human sign-in page for UTP Computing Services. Not a documented API and no machine-readable\n      descriptor was found on the host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/universiti-teknologi-petronas/refs/heads/main/authentication/universiti-teknologi-petronas-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Malaysia
- Private Research University
- Research
- Research Repository
- Institutional Repository
- Open Access
- OAI-PMH
- EPrints
- Identity Federation
- Learning Management
- Scholarly Publishing
---
