---
api_key_in: []
api_specs:
- filename: re-max-eu-datahub-api.postman_collection.json
  format: json
  label: RE/MAX Europe Datahub API
  slug: re-max-eu-datahub-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/re-max/refs/heads/main/collections/re-max-eu-datahub-api.postman_collection.json
- filename: re-max-eu-listings-api.postman_collection.json
  format: json
  label: RE/MAX Europe Listings API
  slug: re-max-eu-listings-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/re-max/refs/heads/main/collections/re-max-eu-listings-api.postman_collection.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Re Max Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: RE/MAX secures its APIs with oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: RE/MAX
provider_slug: re-max
scheme_count: 3
schemes:
- api: RE/MAX Europe Datahub API
  authorizationUrl: https://oauth.datahub.remax.eu/authorize
  client_id_placeholder: Ask_REU
  flow: authorizationCode
  name: datahub-oauth2
  probes:
  - status: 200
    url: https://oauth.datahub.remax.eu/authorize
  - note: 404 to an anonymous GET; the collection documents it as a POST token endpoint
    status: 404
    url: https://oauth.datahub.remax.eu/token
  - status: 404
    url: https://oauth.datahub.remax.eu/.well-known/openid-configuration
  - status: 404
    url: https://oauth.datahub.remax.eu/.well-known/oauth-authorization-server
  scopes: []
  sources:
  - collections/re-max-eu-datahub-api.postman_collection.json
  tokenUrl: https://oauth.datahub.remax.eu/token
  token_transport: access_token query parameter on every request
  type: oauth2
- api: RE/MAX Europe Listings API (staging)
  authorizationUrl: https://oauth.pre-prod.remaxeu-datahub.bwscloud.tech/authorize
  client_id_placeholder: <client-id>
  flow: authorizationCode
  name: listings-oauth2-staging
  probes:
  - note: origin returns nginx 403 to all anonymous paths
    status: 403
    url: https://oauth.pre-prod.remaxeu-datahub.bwscloud.tech/.well-known/openid-configuration
  scopes: []
  sources:
  - collections/re-max-eu-listings-api.postman_collection.json
  tokenUrl: https://oauth.pre-prod.remaxeu-datahub.bwscloud.tech/token
  token_transport: access_token query parameter on every request
  type: oauth2
- anonymous_read: true
  api: RE/MAX Europe Site API (WordPress REST)
  flow: null
  name: wordpress-rest
  probes:
  - note: anonymous read of published content succeeds
    status: 200
    url: https://www.remax.eu/wp-json/wp/v2/posts?per_page=1
  - body: '{"code":"rest_forbidden","message":"Sorry, you are not allowed to do that."}'
    status: 401
    url: https://www.remax.eu/wp-json/wp-abilities/v1/abilities
  - method_probed: POST tools/list
    status: 401
    url: https://www.remax.eu/wp-json/mcp/mcp-adapter-default-server
  sources:
  - well-known/re-max-eu-wp-json.json
  type: cookie-or-application-password
slug: re-max-authentication
source_filename: re-max-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource:\n- collections/re-max-eu-datahub-api.postman_collection.json\n- collections/re-max-eu-listings-api.postman_collection.json\n- https://apidocs.datahub.remax.eu/\n- live anonymous probes of the OAuth and API hosts, 2026-07-26\ndocs: https://apidocs.datahub.remax.eu/\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  api_key_in: []\n  bearer_tokens: false\n  token_transport: query-parameter\n  openid_connect_discovery: false\n  scopes_published: false\n  self_serve_credentials: false\nnote: >-\n  RE/MAX has no single authentication model because it has no single API\n  program. The two documented RE/MAX Europe APIs both use OAuth 2.0\n  authorization code against RE/MAX Europe operated authorization servers, and\n  both carry the resulting token as an access_token QUERY PARAMETER rather than\n  an Authorization header. No OpenID Connect discovery document and no RFC 8414\n  authorization-server metadata\
  \ is served by either authorization server. No\n  scope vocabulary is published; the Postman documentation ships the literal\n  placeholder \"<scope>\". Credentials are not self-serve: the Datahub collection\n  carries the client_id placeholder \"Ask_REU\" (ask RE/MAX Europe). Separately,\n  the remax.eu WordPress estate answers anonymously for public read routes and\n  returns 401 rest_forbidden for everything privileged, including its MCP and\n  Abilities routes.\nschemes:\n- name: datahub-oauth2\n  api: RE/MAX Europe Datahub API\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://oauth.datahub.remax.eu/authorize\n  tokenUrl: https://oauth.datahub.remax.eu/token\n  client_id_placeholder: Ask_REU\n  scopes: []\n  token_transport: access_token query parameter on every request\n  sources:\n  - collections/re-max-eu-datahub-api.postman_collection.json\n  probes:\n  - url: https://oauth.datahub.remax.eu/authorize\n    status: 200\n  - url: https://oauth.datahub.remax.eu/token\n\
  \    status: 404\n    note: 404 to an anonymous GET; the collection documents it as a POST token endpoint\n  - url: https://oauth.datahub.remax.eu/.well-known/openid-configuration\n    status: 404\n  - url: https://oauth.datahub.remax.eu/.well-known/oauth-authorization-server\n    status: 404\n- name: listings-oauth2-staging\n  api: RE/MAX Europe Listings API (staging)\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://oauth.pre-prod.remaxeu-datahub.bwscloud.tech/authorize\n  tokenUrl: https://oauth.pre-prod.remaxeu-datahub.bwscloud.tech/token\n  client_id_placeholder: <client-id>\n  scopes: []\n  token_transport: access_token query parameter on every request\n  sources:\n  - collections/re-max-eu-listings-api.postman_collection.json\n  probes:\n  - url: https://oauth.pre-prod.remaxeu-datahub.bwscloud.tech/.well-known/openid-configuration\n    status: 403\n    note: origin returns nginx 403 to all anonymous paths\n- name: wordpress-rest\n  api: RE/MAX Europe Site API\
  \ (WordPress REST)\n  type: cookie-or-application-password\n  flow: null\n  anonymous_read: true\n  sources:\n  - well-known/re-max-eu-wp-json.json\n  probes:\n  - url: https://www.remax.eu/wp-json/wp/v2/posts?per_page=1\n    status: 200\n    note: anonymous read of published content succeeds\n  - url: https://www.remax.eu/wp-json/wp-abilities/v1/abilities\n    status: 401\n    body: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\"}'\n  - url: https://www.remax.eu/wp-json/mcp/mcp-adapter-default-server\n    status: 401\n    method_probed: 'POST tools/list'\nenforcement_evidence:\n- url: https://api.datahub.remax.eu/external/regions/\n  status: 400\n  body: '{\"status\":[{\"code\":4007,\"message\":\"Login parameter Required\"}],\"result\":{}}'\n  finding: calling without an access_token is rejected\n- url: https://api.datahub.remax.eu/external/regions/?access_token=invalidtoken123\n  status: 403\n  body: '{\"status\":[{\"code\":4004,\"message\":\"Invalid\
  \ or expired Session/Token\"}],\"result\":{}}'\n  finding: an invalid token is rejected; the gate is real and enforced\nsecurity_observations:\n- >-\n  Bearer material in the query string. Both RE/MAX Europe APIs pass the OAuth\n  access token as a URL query parameter, so tokens land in server logs, proxy\n  logs, referrer headers and browser history. An Authorization header is the\n  RFC 6750 recommended transport.\n- >-\n  No authorization-server metadata. Neither OIDC discovery nor RFC 8414 metadata\n  is served, so a client cannot machine-discover endpoints, supported grants,\n  PKCE support or signing keys.\n- >-\n  No published scopes. Without a scope vocabulary, every issued credential is\n  effectively coarse-grained from a consumer's point of view.\n- >-\n  The published staging Listings collection embedded a live-looking 128-character\n  hexadecimal access_token in four request URLs; those values were redacted\n  before this repo saved the file (see review.yml harvest.collections).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/re-max/refs/heads/main/authentication/re-max-authentication.yml
summary_line: oauth2 · 3 schemes
tags:
- Real Estate
- United States
- Brokerage
- Property Listings
- MLS
- RESO
- IDX
- PropTech
- Franchising
- Mortgage
- Rentals
---
