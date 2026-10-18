---
anonymous_access: false
api_key_in: []
api_specs:
- filename: yoti-accounts-api-openapi.yml
  format: yaml
  label: Yoti Accounts API
  slug: yoti-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoti/refs/heads/main/openapi/yoti-accounts-api-openapi.yml
- filename: yoti-ai-api-openapi.yml
  format: yaml
  label: Yoti AI API
  slug: yoti-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoti/refs/heads/main/openapi/yoti-ai-api-openapi.yml
- filename: yoti-oauth-api-openapi.yml
  format: yaml
  label: Yoti OAuth API
  slug: yoti-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoti/refs/heads/main/openapi/yoti-oauth-api-openapi.yml
- filename: yoti-path-api-openapi.yml
  format: yaml
  label: Yoti Path API
  slug: yoti-path-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoti/refs/heads/main/openapi/yoti-path-api-openapi.yml
- filename: yoti-poa-api-openapi.yml
  format: yaml
  label: Yoti Poa API
  slug: yoti-poa-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoti/refs/heads/main/openapi/yoti-poa-api-openapi.yml
- filename: yoti-sessions-api-openapi.yml
  format: yaml
  label: Yoti Sessions API
  slug: yoti-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoti/refs/heads/main/openapi/yoti-sessions-api-openapi.yml
auth_types: []
description: Yoti uses OAuth2 client‑credentials flow with a JWT client assertion and also supports RSA‑signed request headers for certain APIs.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Yoti Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yoti declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Yoti
provider_slug: yoti
scheme_count: 2
schemes:
- evidence: All API calls will be made using an OAuth Access Token as a bearer token.
  how_to_obtain: Generate a JWT signed with the service/SDK private PEM key (PS384 algorithm) and use it as a client assertion in a POST request to the token URL to obtain an access token. The JWT must contain the required claims (iss, sub, aud, jti, exp, iat).
  name: OAuth2 Client Credentials
  scopes:
  - did:match
  - poa:verify
  token_url: https://auth.api.yoti.com/v1/oauth/token
  type: oauth2
- evidence: Yoti API endpoints are authenticated through signed requests, and the current approach for building signed requests consists of passing the following HTTP Headers
  header: X-Yoti-Auth-Digest
  how_to_obtain: Compute the digest by concatenating HTTP method, path, query string (including nonce and timestamp) and base64‑encoded body with '&', sign the string with SHA256withRSA using the PEM private key, then Base64‑encode the signature. Include the result in the X‑Yoti‑Auth‑Digest header and the SDK ID in X‑Yoti‑Auth‑Id.
  location: header
  name: RSA‑signed request headers
  type: other
slug: yoti-authentication
source_filename: yoti-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.yoti.com/digital-id/did-match-authentication.md
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.yoti.com/digital-id/did-match-authentication.md\nsources:\n- https://developers.yoti.com/digital-id/did-match-authentication.md\n- https://developers.yoti.com/age-estimation/api-authentication.md\n- https://developers.yoti.com/proof-of-age/api-authentication.md\n- https://developers.yoti.com/age-verification/age-token.md\ndescription: Yoti uses OAuth2 client‑credentials flow with a JWT client assertion and also supports RSA‑signed request headers for certain APIs.\nschemes:\n- type: oauth2\n  name: OAuth2 Client Credentials\n  evidence: All API calls will be made using an OAuth Access Token as a bearer token.\n  token_url: https://auth.api.yoti.com/v1/oauth/token\n  scopes:\n  - did:match\n  - poa:verify\n  how_to_obtain: Generate a JWT signed with the service/SDK private PEM key (PS384 algorithm) and use it as a client assertion in a POST request\n    to the\
  \ token URL to obtain an access token. The JWT must contain the required claims (iss, sub, aud, jti, exp, iat).\n- type: other\n  name: RSA‑signed request headers\n  evidence: Yoti API endpoints are authenticated through signed requests, and the current approach for building signed requests consists of passing\n    the following HTTP Headers\n  location: header\n  header: X-Yoti-Auth-Digest\n  how_to_obtain: Compute the digest by concatenating HTTP method, path, query string (including nonce and timestamp) and base64‑encoded body with\n    '&', sign the string with SHA256withRSA using the PEM private key, then Base64‑encode the signature. Include the result in the X‑Yoti‑Auth‑Digest\n    header and the SDK ID in X‑Yoti‑Auth‑Id.\ndocs: https://developers.yoti.com/digital-id/did-match-authentication.md\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoti/refs/heads/main/authentication/yoti-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Identity
- Verification
- DigitalID
- SDK
---
