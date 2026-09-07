---
anonymous_access: false
api_key_in:
- header
- query
api_specs:
- filename: elsevier-scopus-swagger.json
  format: json
  label: Elsevier Scopus APIs
  slug: elsevier-scopus-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-scopus-swagger.json
- filename: elsevier-sciencedirect-swagger.json
  format: json
  label: Elsevier ScienceDirect APIs
  slug: elsevier-sciencedirect-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-sciencedirect-swagger.json
- filename: elsevier-scival-swagger.json
  format: json
  label: Elsevier SciVal API
  slug: elsevier-scival-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-scival-swagger.json
- filename: elsevier-engineering-village-swagger.json
  format: json
  label: Elsevier Engineering Village API
  slug: elsevier-engineering-village-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-engineering-village-swagger.json
- filename: elsevier-retrieval-swagger.json
  format: json
  label: Elsevier Retrieval APIs
  slug: elsevier-retrieval-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-retrieval-swagger.json
- filename: elsevier-metadata-swagger.json
  format: json
  label: Elsevier Metadata APIs
  slug: elsevier-metadata-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-metadata-swagger.json
- filename: elsevier-abstract-api-openapi.yml
  format: yaml
  label: Elsevier Abstract API
  slug: elsevier-abstract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-abstract-api-openapi.yml
- filename: elsevier-search-api-openapi.yml
  format: yaml
  label: Elsevier Search API
  slug: elsevier-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/openapi/elsevier-search-api-openapi.yml
auth_types:
- apiKey
- bearer-like-token
- oauth2
description: 'Elsevier layers four things that all get called "authentication": an API key that identifies the APPLICATION, and then three different ways of establishing WHICH CUSTOMER ACCOUNT the call is entitled to read as. The key alone gets you almost nothing — entitlement is resolved from institutional IP address, an authtoken, or an insttoken. An agent running outside an institutional network will authenticate successfully and still be refused content, and that is the single most misread thing about this API.'
kind: authentication
layout: security
mechanism_count: 6
method: searched
name: Elsevier Authentication
name_suffix: Authentication
oauth_flows: []
overview: Elsevier secures its APIs with apiKey, bearer-like-token, and oauth2 across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Elsevier
provider_slug: elsevier
scheme_count: 6
schemes:
- description: Required on every request to every API. Registered self-serve at https://dev.elsevier.com/apikey/manage.
  in: header
  name: apiKey
  observed_in_wadl_methods: 122
  parameter: X-ELS-APIKey
  required: true
  type: apiKey
- description: Elsevier documents the key as a URL query parameter as an explicit alternative to the header, and its own portal examples embed it that way in <object>/<iframe> tags.
  in: query
  name: apiKeyQuery
  observed_in_wadl_methods: 123
  parameter: apiKey
  required: false
  risk: Credentials in the query string are logged by intermediaries and land in browser history and referrers. This is the one place the Elsevier contract fails the credentials-not-in-query test, and it fails it because the provider recommends it.
  type: apiKey
- description: Obtained from the Authentication API (GET https://api.elsevier.com/authenticate?platform=SCOPUS), which resolves the caller to one customer account when the source IP maps to more than one. The response either returns an authtoken or a <pathChoices> list to pick from with &choice=.
  in: header
  name: authtoken
  observed_in_wadl_methods: 110
  parameter: X-ELS-Authtoken
  required: false
  ttl: 2h
  ttl_source: '"An authtoken expires two hours after issuance by the Authentication API." — dev.elsevier.com/tecdoc_api_authentication.html'
  type: apiKey
- description: A proprietary Institutional Token issued by Elsevier's integration support team for remote access outside the institutional network. Not self-serve — it must be requested.
  in: header
  name: insttoken
  observed_in_wadl_methods: 106
  parameter: X-ELS-Insttoken
  required: false
  restrictions:
  - Must be kept server-side in a password-protected environment.
  - Must never appear in browser-side code or in the address bar.
  - Represents full access to a customer account and may be revoked at any time without notice.
  - All requests using an insttoken must be over HTTPS.
  type: apiKey
- description: An Authorization header is declared on 110 of the 138 WADL methods. Elsevier's auth guide describes "Using OAuth. We offer an oauth implementation for developers wanting to integrate ScienceDirect and/or Scopus content into client-side applications requiring access to user level (rather than institutional) content."
  gap: 'No authorization endpoint, token endpoint, grant type, client-registration flow or scope list is published anywhere on dev.elsevier.com. UPDATED 2026-09-06: the endpoints do exist and are discoverable — https://id.elsevier.com serves both an OpenID Connect discovery document and RFC 8414 authorization-server metadata anonymously (see oauth_discovery below and scopes/elsevier-scopes.yml) — but nothing on the developer portal or the API host names that server, and none of its 35 advertised scopes governs a Research Products API operation. The route from a 401 on api.elsevier.com to that token endpoint has to be guessed.'
  name: authorization
  parameter: Authorization
  required: false
  scheme: bearer
  type: http
- description: Crossref Text and Data Mining client token, accepted on the article/object retrieval surface alongside CR-Clickthrough-Client-Token. A cross-publisher standard, not an Elsevier-proprietary one.
  in: header
  name: crossref-tdm
  observed_in_wadl_methods: 5
  parameter: CR-TDM-Client-Token
  required: false
  type: apiKey
slug: elsevier-authentication
source_filename: elsevier-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://dev.elsevier.com/tecdoc_api_authentication.html\ndocs: https://dev.elsevier.com/tecdoc_api_authentication.html\nsupporting_sources:\n- openapi/elsevier-scopus-swagger.json (and the six sibling Swagger 2.0 documents harvested from dev.elsevier.com/elsdoc/)\n- wadl/ (37 first-party WADL contracts; header parameters counted across 138 methods)\n- https://dev.elsevier.com/support.html\n- live probe of https://api.elsevier.com/content/search/scopus, unauthenticated, 2026-09-06\ndescription: >-\n  Elsevier layers four things that all get called \"authentication\": an API key that identifies\n  the APPLICATION, and then three different ways of establishing WHICH CUSTOMER ACCOUNT the\n  call is entitled to read as. The key alone gets you almost nothing — entitlement is resolved\n  from institutional IP address, an authtoken, or an insttoken. An agent running outside an\n  institutional network will authenticate successfully\
  \ and still be refused content, and that\n  is the single most misread thing about this API.\nsummary:\n  types:\n  - apiKey\n  - bearer-like-token\n  - oauth2\n  api_key_in:\n  - header\n  - query\n  entitlement_model: institutional\n  scopes_published: false\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-ELS-APIKey\n  required: true\n  description: >-\n    Required on every request to every API. Registered self-serve at\n    https://dev.elsevier.com/apikey/manage.\n  observed_in_wadl_methods: 122\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apiKey\n  required: false\n  description: >-\n    Elsevier documents the key as a URL query parameter as an explicit alternative to the\n    header, and its own portal examples embed it that way in <object>/<iframe> tags.\n  observed_in_wadl_methods: 123\n  risk: >-\n    Credentials in the query string are logged by intermediaries and land in browser history\n    and referrers. This is the one place the\
  \ Elsevier contract fails the\n    credentials-not-in-query test, and it fails it because the provider recommends it.\n- name: authtoken\n  type: apiKey\n  in: header\n  parameter: X-ELS-Authtoken\n  required: false\n  description: >-\n    Obtained from the Authentication API (GET https://api.elsevier.com/authenticate?platform=SCOPUS),\n    which resolves the caller to one customer account when the source IP maps to more than one.\n    The response either returns an authtoken or a <pathChoices> list to pick from with &choice=.\n  ttl: 2h\n  ttl_source: >-\n    \"An authtoken expires two hours after issuance by the Authentication API.\" —\n    dev.elsevier.com/tecdoc_api_authentication.html\n  observed_in_wadl_methods: 110\n- name: insttoken\n  type: apiKey\n  in: header\n  parameter: X-ELS-Insttoken\n  required: false\n  description: >-\n    A proprietary Institutional Token issued by Elsevier's integration support team for remote\n    access outside the institutional network. Not self-serve\
  \ — it must be requested.\n  restrictions:\n  - Must be kept server-side in a password-protected environment.\n  - Must never appear in browser-side code or in the address bar.\n  - Represents full access to a customer account and may be revoked at any time without notice.\n  - All requests using an insttoken must be over HTTPS.\n  observed_in_wadl_methods: 106\n- name: authorization\n  type: http\n  scheme: bearer\n  parameter: Authorization\n  required: false\n  description: >-\n    An Authorization header is declared on 110 of the 138 WADL methods. Elsevier's auth guide\n    describes \"Using OAuth. We offer an oauth implementation for developers wanting to integrate\n    ScienceDirect and/or Scopus content into client-side applications requiring access to user\n    level (rather than institutional) content.\"\n  gap: >-\n    No authorization endpoint, token endpoint, grant type, client-registration flow or scope\n    list is published anywhere on dev.elsevier.com. UPDATED 2026-09-06:\
  \ the endpoints do\n    exist and are discoverable — https://id.elsevier.com serves both an OpenID Connect\n    discovery document and RFC 8414 authorization-server metadata anonymously (see\n    oauth_discovery below and scopes/elsevier-scopes.yml) — but nothing on the developer\n    portal or the API host names that server, and none of its 35 advertised scopes governs a\n    Research Products API operation. The route from a 401 on api.elsevier.com to that token\n    endpoint has to be guessed.\n- name: crossref-tdm\n  type: apiKey\n  in: header\n  parameter: CR-TDM-Client-Token\n  required: false\n  description: >-\n    Crossref Text and Data Mining client token, accepted on the article/object retrieval\n    surface alongside CR-Clickthrough-Client-Token. A cross-publisher standard, not an\n    Elsevier-proprietary one.\n  observed_in_wadl_methods: 5\noauth_discovery:\n  found: true\n  method: probed\n  probed: '2026-09-06'\n  issuer: https://id.elsevier.com\n  software: PingFederate\n\
  \  how_found: >-\n    https://dev.elsevier.com/apikey/manage returns 302 to\n    https://id.elsevier.com/as/authorization.oauth2 with client_id ELSAPI-PROD and a scope\n    list including urn:idp:policy:product:confirmation:EAPI:emailconfirmation. EAPI is the\n    developer portal. The host was then probed directly.\n  documents:\n  - url: https://id.elsevier.com/.well-known/openid-configuration\n    status: 200\n    file: ../well-known/elsevier-id-openid-configuration.json\n  - url: https://id.elsevier.com/.well-known/oauth-authorization-server\n    status: 200\n    file: ../well-known/elsevier-id-oauth-authorization-server.json\n  - url: https://api.elsevier.com/.well-known/oauth-protected-resource\n    status: 404\n  endpoints:\n    authorization: https://id.elsevier.com/as/authorization.oauth2\n    token: https://id.elsevier.com/as/token.oauth2\n    introspection: https://id.elsevier.com/as/introspect.oauth2\n    revocation: https://id.elsevier.com/as/revoke_token.oauth2\n    userinfo:\
  \ https://id.elsevier.com/idp/userinfo.openid\n    registration: https://id.elsevier.com/as/clients.oauth2\n    device_authorization: https://id.elsevier.com/as/device_authz.oauth2\n    jwks: https://id.elsevier.com/pf/JWKS\n  pkce: [plain, S256]\n  scopes: see scopes/elsevier-scopes.yml\n  scope_count: 35\n  applies_to: >-\n    Elsevier account identity across its web products (ScienceDirect, SciVal, Pure, Mendeley,\n    and the developer portal sign-in). NOT the Research Products APIs on api.elsevier.com,\n    which remain key-plus-entitlement. Do not read this discovery document as an authorization\n    model for the content APIs.\n  weaknesses:\n  - implicit and password grants still advertised\n  - id_token_signing_alg_values_supported includes \"none\"\n  - no oauth-protected-resource document on the API host to link the two\nentitlement:\n  primary: institutional-ip\n  description: >-\n    \"Elsevier Research Products APIs rely primarily on Institutional IP address for\n    authentication.\
  \ API access through proxies is not supported.\" Content returned is scoped\n    to the subscriptions of whichever account the IP resolves to.\n  failure_mode: >-\n    A valid key called from outside the institutional network returns 401/403 with\n    X-ELS-Status AUTHENTICATION_ERROR or an entitlement error — indistinguishable at the status\n    code from a bad key. The X-ELS-Status header is the only thing that separates them.\n  remote_access: Institutional Token (X-ELS-Insttoken), by request only.\nerror_signals:\n  header: X-ELS-Status\n  observed:\n  - value: AUTHENTICATION_ERROR - Invalid API Key\n    status: 401\n    probed: 'https://api.elsevier.com/content/search/scopus?query=heart (no key), 2026-09-06'\n  envelope: '{\"service-error\":{\"status\":{\"statusCode\":\"...\",\"statusText\":\"...\"}}}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/elsevier/refs/heads/main/authentication/elsevier-authentication.yml
summary_line: apiKey/bearer-like-token/oauth2 · 6 schemes
tags:
- Content
- Journals
- Medical
- Research
- Scientific
- Technical
---
