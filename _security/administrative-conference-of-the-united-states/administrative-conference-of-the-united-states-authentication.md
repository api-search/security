---
api_key_in: []
auth_types: []
description: 'ACUS runs one publicly callable API surface: the MediaWiki Action API and MediaWiki REST API v1 behind the Federal Administrative Procedure Sourcebook wiki at sourcebook.acus.gov. All read operations are ANONYMOUS — no API key, no token, no account. There are no OAuth flows: the wiki''s own RSD document reports OAuth=false. Write actions exist in the module list but require a wiki account and a CSRF token, and account creation is not open to the public. The other two ACUS data properties (the EAJA Awards Database and the Federal Administrative Adjudication Database) expose no programmatic interface at all, so they have no auth model.'
kind: authentication
layout: security
method: probed
name: Administrative Conference Of The United States Authentication
name_suffix: Authentication
oauth_flows: []
overview: Administrative Conference of the United States declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Administrative Conference of the United States
provider_slug: administrative-conference-of-the-united-states
scheme_count: 0
schemes: []
slug: administrative-conference-of-the-united-states-authentication
source_filename: administrative-conference-of-the-united-states-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  live anonymous requests to https://sourcebook.acus.gov/api.php and\n  https://sourcebook.acus.gov/rest.php/v1/* on 2026-08-30, plus\n  https://sourcebook.acus.gov/api.php?action=rsd\nprovider: Administrative Conference of the United States\nproviderId: administrative-conference-of-the-united-states\ndescription: >-\n  ACUS runs one publicly callable API surface: the MediaWiki Action API and MediaWiki\n  REST API v1 behind the Federal Administrative Procedure Sourcebook wiki at\n  sourcebook.acus.gov. All read operations are ANONYMOUS — no API key, no token, no\n  account. There are no OAuth flows: the wiki's own RSD document reports\n  OAuth=false. Write actions exist in the module list but require a wiki account and a\n  CSRF token, and account creation is not open to the public. The other two ACUS data\n  properties (the EAJA Awards Database and the Federal Administrative Adjudication\n  Database) expose no programmatic\
  \ interface at all, so they have no auth model.\napis:\n  - name: Federal Administrative Procedure Sourcebook API\n    baseURL: https://sourcebook.acus.gov/api.php\n    rest_baseURL: https://sourcebook.acus.gov/rest.php/v1\n    schemes:\n      - id: anonymous\n        type: none\n        applies_to: all read operations (action=query, action=parse, action=opensearch, REST GET)\n        in: n/a\n        evidence: >-\n          GET https://sourcebook.acus.gov/api.php?action=query&meta=siteinfo&format=json -> 200\n          with no credentials; GET https://sourcebook.acus.gov/rest.php/v1/page/Main_Page -> 200\n          with no credentials.\n      - id: mediawiki-session-csrf\n        type: cookie+csrf-token\n        applies_to: >-\n          write modules (edit, upload, move, delete, protect, patrol, watch, options,\n          visualeditoredit and the rest of the 54-action surface)\n        in: cookie\n        token_endpoint: https://sourcebook.acus.gov/api.php?action=query&meta=tokens\n\
  \        evidence: >-\n          MediaWiki 1.43.0 standard model, reported by action=paraminfo&modules=main. Not\n          exercised — this repo issues read-only probes only.\n        note: >-\n          Not an agent-usable auth model. There is no self-service registration for the\n          Sourcebook wiki, and action=rsd reports OAuth false, so no OAuth/OAuth2\n          consumer flow is available.\n      - id: oauth\n        type: oauth2\n        available: false\n        evidence: >-\n          GET https://sourcebook.acus.gov/api.php?action=rsd -> 200,\n          <setting name=\"OAuth\">false</setting>. No OAuth extension is installed\n          (siprop=extensions returns only skins plus VisualEditor, WikiEditor, Cite).\naccess_control_findings:\n  - finding: user-agent-gated\n    severity: high-for-agents\n    detail: >-\n      Every acus.gov host returns HTTP 403 to non-browser user agents. Measured 2026-08-30\n      against https://sourcebook.acus.gov/rest.php/v1/page/Main_Page:\
  \ curl/8.7.1 -> 403,\n      python-requests/2.31.0 -> 403, GPTBot/1.0 -> 403, desktop Chrome UA -> 200. The\n      identical pattern holds for www.acus.gov and for the Action API. The API is public\n      and unauthenticated, but a default-configured HTTP client or crawler cannot reach it\n      without spoofing a browser User-Agent. This is an edge policy, not an auth\n      requirement, and it is the single biggest barrier to agent consumption of ACUS data.\n    evidence:\n      - request: 'GET https://sourcebook.acus.gov/rest.php/v1/page/Main_Page (UA: curl/8.7.1)'\n        status: 403\n      - request: 'GET https://sourcebook.acus.gov/rest.php/v1/page/Main_Page (UA: GPTBot/1.0)'\n        status: 403\n      - request: 'GET https://sourcebook.acus.gov/rest.php/v1/page/Main_Page (UA: Chrome 126 desktop)'\n        status: 200\nwell_known:\n  openid_configuration: null\n  oauth_authorization_server: null\n  note: Both probed on www.acus.gov and returned 404 — see well-known/ artifact.\n\
  maintainers:\n  - FN: Kin Lane\n    X-twitter: apievangelist\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/administrative-conference-of-the-united-states/refs/heads/main/authentication/administrative-conference-of-the-united-states-authentication.yml
summary_line: 0 schemes
tags:
- Federal-Government
- Regulatory Reform
- Administrative Law
- Government Efficiency
- Open Data
- Policy Research
---
