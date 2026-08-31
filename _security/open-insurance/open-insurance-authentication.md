---
api_key_in:
- body
- query
- sdk-initialiser
api_specs:
- filename: open-insurance-policy-api-openapi.yml
  format: yaml
  label: Open Policy API
  slug: open-insurance-policy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/open-insurance/refs/heads/main/openapi/open-insurance-policy-api-openapi.yml
auth_types:
- apiKey
- jwt-bearer (deprecated)
description: ''
kind: authentication
layout: security
method: searched
name: Open Insurance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Open secures its APIs with apiKey and jwt-bearer (deprecated) across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Open
provider_slug: open-insurance
scheme_count: 5
schemes:
- applies_to:
  - openapi/open-insurance-certificate-of-currency-openapi.json#coc
  description: The Certificate of Currency operation takes the api_key and api_secret as fields in the JSON request body rather than in a header. Both are required alongside policy_number.
  docs: https://developers.beopen.com/reference/coc
  documented_in_spec: false
  in: body
  name: api_key_secret_body
  parameters:
  - api_key
  - api_secret
  type: apiKey
- applies_to:
  - opensdk.load
  description: Open.js is initialised with the partner API key — opensdk.load("YOUR_API_KEY"). The optional sandbox flag repoints the library at api.sandbox.beopen.com and the sandbox portal.
  docs: https://developers.beopen.com/docs/using-openjs
  in: sdk-initialiser
  name: api_key_sdk
  parameters:
  - apiKey
  type: apiKey
- applies_to:
  - URL Handover
  - Open.Widget iframe src
  description: The redirect and embed surfaces carry the API key as the `key` query parameter, e.g. https://stage.huddle.com.au/?key=API_KEY&pc=PRODUCT_CODE.
  docs: https://developers.beopen.com/docs/basic-redirection
  in: query
  name: api_key_query
  parameters:
  - key
  type: apiKey
- algorithm: HS256
  bearerFormat: JWT
  deprecation_note: '"This feature has been deprecated and should not be used in new implementation!" — verbatim from the docs page.'
  description: 'An HS256 JWT signed with the account secret key unlocks advanced SDK workflows (customer_ref linking, resume-quote). Passed as the authToken option to opensdk.load, or as the `jwt` query parameter on a URL Handover. Payload documented as {"customer_ref": "123"}.'
  docs: https://developers.beopen.com/docs/authenticating-using-jwt
  name: jwt_hs256
  scheme: bearer
  status: deprecated
  type: http
- applies_to:
  - https://developers.beopen.com/mcp
  authorization_servers:
  - https://dash.readme.com/oidc
  description: Third-party. The developer hub's MCP endpoint is protected by ReadMe's own OIDC authorization server, advertised via RFC 9728 metadata at /.well-known/oauth-protected-resource/mcp. This is documentation-platform auth, not Open API auth.
  first_party: false
  name: readme_oidc_mcp
  scope: documentation MCP endpoint only
  type: oauth2
slug: open-insurance-authentication
source_filename: open-insurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: openapi/open-insurance-certificate-of-currency-openapi.json\ndocs: https://developers.beopen.com/docs/keys\nnote: >-\n  The harvested OpenAPI declares an EMPTY components.securitySchemes and an empty\n  security requirement, so mechanical derivation yields nothing — the credential\n  model lives entirely in prose and in the request body schema. Captured here from\n  the docs. Credentials are partner-issued: \"Keys are issued by Open during\n  account creation. Contact your account manager or email sales@beopen.com.\"\n  There is no self-serve signup, no OAuth and no OpenID Connect anywhere on Open's\n  own hosts (openid-configuration and oauth-authorization-server return 404 on\n  api.beopen.com, developers.beopen.com and www.beopen.com).\nsummary:\n  types:\n  - apiKey\n  - jwt-bearer (deprecated)\n  api_key_in:\n  - body\n  - query\n  - sdk-initialiser\n  oauth2_flows: []\n  self_serve: false\n  environments:\n  - sandbox\n\
  \  - production\n  key_pair: api key + secret key, one pair per environment\nschemes:\n- name: api_key_secret_body\n  type: apiKey\n  in: body\n  parameters:\n  - api_key\n  - api_secret\n  applies_to:\n  - openapi/open-insurance-certificate-of-currency-openapi.json#coc\n  description: >-\n    The Certificate of Currency operation takes the api_key and api_secret as\n    fields in the JSON request body rather than in a header. Both are required\n    alongside policy_number.\n  documented_in_spec: false\n  docs: https://developers.beopen.com/reference/coc\n- name: api_key_sdk\n  type: apiKey\n  in: sdk-initialiser\n  parameters:\n  - apiKey\n  applies_to:\n  - opensdk.load\n  description: >-\n    Open.js is initialised with the partner API key — opensdk.load(\"YOUR_API_KEY\").\n    The optional sandbox flag repoints the library at api.sandbox.beopen.com and\n    the sandbox portal.\n  docs: https://developers.beopen.com/docs/using-openjs\n- name: api_key_query\n  type: apiKey\n  in: query\n\
  \  parameters:\n  - key\n  applies_to:\n  - URL Handover\n  - Open.Widget iframe src\n  description: >-\n    The redirect and embed surfaces carry the API key as the `key` query\n    parameter, e.g. https://stage.huddle.com.au/?key=API_KEY&pc=PRODUCT_CODE.\n  docs: https://developers.beopen.com/docs/basic-redirection\n- name: jwt_hs256\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  algorithm: HS256\n  status: deprecated\n  deprecation_note: >-\n    \"This feature has been deprecated and should not be used in new\n    implementation!\" — verbatim from the docs page.\n  description: >-\n    An HS256 JWT signed with the account secret key unlocks advanced SDK\n    workflows (customer_ref linking, resume-quote). Passed as the authToken\n    option to opensdk.load, or as the `jwt` query parameter on a URL Handover.\n    Payload documented as {\"customer_ref\": \"123\"}.\n  docs: https://developers.beopen.com/docs/authenticating-using-jwt\n- name: readme_oidc_mcp\n  type: oauth2\n \
  \ scope: documentation MCP endpoint only\n  authorization_servers:\n  - https://dash.readme.com/oidc\n  applies_to:\n  - https://developers.beopen.com/mcp\n  description: >-\n    Third-party. The developer hub's MCP endpoint is protected by ReadMe's own\n    OIDC authorization server, advertised via RFC 9728 metadata at\n    /.well-known/oauth-protected-resource/mcp. This is documentation-platform\n    auth, not Open API auth.\n  first_party: false\nkey_management:\n  issuance: Open account manager / sales@beopen.com at partner account creation\n  rotation: not documented\n  self_serve_console: false\n  guidance: >-\n    Docs advise storing keys in a password manager or secrets service, keeping\n    them out of source control, and treating public exposure as an account\n    compromise (\"A user might abuse API calls or create insurance quotes on\n    behalf of your account\").\n  docs: https://developers.beopen.com/docs/keys\ngaps:\n- The OpenAPI does not declare any securityScheme, so\
  \ generated clients get no auth wiring.\n- Credentials travel in the request body, which excludes them from standard Authorization-header tooling and proxy redaction.\n- No documented key rotation, expiry or revocation procedure.\n- No OAuth 2.0 / OIDC option for partner or end-user delegated access.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/open-insurance/refs/heads/main/authentication/open-insurance-authentication.yml
summary_line: apiKey/jwt-bearer (deprecated) · 5 schemes
tags:
- Insurance
- Australia
- Insurtech
- Embedded Insurance
- Property and Casualty
- Travel Insurance
- Underwriting
- Policy Administration
- White Label
- Quotes
---
