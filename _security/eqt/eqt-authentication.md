---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Eqt Authentication
name_suffix: Authentication
oauth_flows: []
overview: EQT Corporation declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: EQT Corporation
provider_slug: eqt
scheme_count: 0
schemes: []
slug: eqt-authentication
source_filename: eqt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: https://infopost.eqt.com/.well-known/openid-configuration (200) and https://customers.equitransmidstream.com/.well-known/openid-configuration\n  (200), fetched anonymously 2026-09-06; JWKS confirmed at https://infopost.eqt.com/id/keys (200)\nnote: EQT Corporation publishes no public API and therefore no API authentication documentation. What\n  it does serve are two working OpenID Connect authorization servers fronting its customer portals. These\n  are Salesforce Experience Cloud identity endpoints running under EQT-controlled hostnames — the authorization\n  surface belongs to EQT, the implementation is Salesforce's. Access is limited to registered pipeline\n  customers; there is no self-service signup and no documented programmatic onboarding. Nothing here was\n  derived from an OpenAPI spec, because no spec exists.\nsummary:\n  public_api: false\n  schemes:\n  - openIdConnect\n  - oauth2\n  self_service_signup: false\n  documentation_url:\
  \ null\nproviders:\n- name: EQT Midstream Informational Postings / Customer Portal\n  host: infopost.eqt.com\n  issuer: https://infopost.eqt.com\n  type: openIdConnect\n  discovery: https://infopost.eqt.com/.well-known/openid-configuration\n  discovery_status: 200\n  jwks_uri: https://infopost.eqt.com/id/keys\n  jwks_status: 200\n  authorization_endpoint: https://infopost.eqt.com/services/oauth2/authorize\n  token_endpoint: https://infopost.eqt.com/services/oauth2/token\n  userinfo_endpoint: https://infopost.eqt.com/services/oauth2/userinfo\n  revocation_endpoint: https://infopost.eqt.com/services/oauth2/revoke\n  introspection_endpoint: https://infopost.eqt.com/services/oauth2/introspect\n  registration_endpoint: https://infopost.eqt.com/services/oauth2/register\n  registration_open: false\n  registration_probe:\n    url: https://infopost.eqt.com/services/oauth2/register\n    status: 401\n    body: '{\"error\":\"invalid_client\",\"error_description\":\"invalid client credentials\"}'\n\
  \    note: dynamic client registration is advertised in the discovery document but rejects anonymous callers,\n      so it is not an open DCR surface\n  response_types_supported:\n  - code\n  - token\n  - token id_token\n  id_token_signing_alg_values_supported:\n  - RS256\n  platform: Salesforce Experience Cloud\n- name: Equitrans Midstream Customer Portal\n  host: customers.equitransmidstream.com\n  issuer: https://customers.equitransmidstream.com/CustomerPortal\n  type: openIdConnect\n  discovery: https://customers.equitransmidstream.com/.well-known/openid-configuration\n  discovery_status: 200\n  jwks_uri: https://customers.equitransmidstream.com/CustomerPortal/id/keys\n  jwks_status: 200\n  authorization_endpoint: https://customers.equitransmidstream.com/CustomerPortal/services/oauth2/authorize\n  token_endpoint: https://customers.equitransmidstream.com/CustomerPortal/services/oauth2/token\n  userinfo_endpoint: https://customers.equitransmidstream.com/CustomerPortal/services/oauth2/userinfo\n\
  \  revocation_endpoint: https://customers.equitransmidstream.com/CustomerPortal/services/oauth2/revoke\n  introspection_endpoint: https://customers.equitransmidstream.com/CustomerPortal/services/oauth2/introspect\n  registration_endpoint: https://customers.equitransmidstream.com/CustomerPortal/services/oauth2/register\n  registration_open: false\n  response_types_supported:\n  - code\n  - token\n  - token id_token\n  id_token_signing_alg_values_supported:\n  - RS256\n  platform: Salesforce Experience Cloud\n  ownership_note: Equitrans Midstream has been a wholly owned subsidiary of EQT Corporation since the\n    acquisition closed 22 July 2024, so this host is in scope for the EQT record.\ngaps:\n- no public API authentication documentation page exists\n- no API keys, no developer credentials, no self-service credential issuance\n- the OIDC surfaces are portal sign-in for contracted pipeline customers, not an API auth model\nscopes_advertised:\n  count: 36\n  identical_across_both_servers:\
  \ true\n  note: These are the stock Salesforce Experience Cloud scope values advertised by scopes_supported in\n    both discovery documents. They are NOT a scope model EQT designed, and EQT documents no OAuth scope\n    reference anywhere. Recorded here as observed metadata rather than as a scopes/ artifact, because\n    no OpenAPI declares oauth2 and no EQT documentation covers OAuth — the two conditions the enrichment\n    contract requires before a scopes artifact may be written.\n  values:\n  - address\n  - api\n  - cdp_api\n  - cdp_calculated_insight_api\n  - cdp_identityresolution_api\n  - cdp_ingest_api\n  - cdp_profile_api\n  - cdp_query_api\n  - cdp_segment_api\n  - chatbot_api\n  - chatter_api\n  - content\n  - custom_permissions\n  - data_cloud_user_claims\n  - eclair_api\n  - einstein_gpt_api\n  - email\n  - forgot_password\n  - full\n  - id\n  - interaction_api\n  - lightning\n  - mcp_api\n  - offline_access\n  - openid\n  - pardot_api\n  - phone\n  - profile\n  - pwdless_login_api\n\
  \  - refresh_token\n  - scrt_api\n  - sfap_api\n  - user_registration_api\n  - visualforce\n  - wave_api\n  - web\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eqt/refs/heads/main/authentication/eqt-authentication.yml
summary_line: 0 schemes
tags:
- Energy
- Natural Gas
- Oil and Gas
- Appalachian Basin
- Fortune 1000
---
