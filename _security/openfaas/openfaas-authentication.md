---
anonymous_access: false
api_key_in: []
api_specs:
- filename: openfaas-openapi-generated.yml
  format: yaml
  label: OpenFaaS API
  slug: openfaas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openfaas/refs/heads/main/openapi/_ae-authored/openfaas-openapi-generated.yml
auth_types: []
description: Authentication methods documented for OpenFaaS functions
kind: authentication
layout: security
mechanism_count: 4
method: searched
name: Openfaas Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenFaaS declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: OpenFaaS
provider_slug: openfaas
scheme_count: 4
schemes:
- evidence: You can also create and manage your own Bearer tokens or API keys. These are simply shared secrets, where the client (the user or machine invoking the function) and the server (the function) share a copy of the token.
  header: Authorization
  how_to_obtain: Create a token as a secret and assign it to the function; the client then sends it in the Authorization header.
  location: header
  name: Bearer token
  type: http-bearer
- evidence: 'You can enable basic-authentication for a web-portal or an API by setting the appropriate header such as WWW-Authenticate: Basic realm="User Visible Realm" . This is the approach that the OpenFaaS gateway takes, and the OpenFaaS Pro edition comes with an OIDC integration.'
  header: Authorization
  how_to_obtain: Configure the gateway with a username and password; clients provide credentials using the HTTP Basic scheme.
  location: header
  name: Basic authentication
  type: http-basic
- evidence: When functions receive webhooks, most publishers of events will not support any form of authentication. Messages are verified using symmetric keys, where the client (your function) and the server (GitHub, Stripe, YouTube, etc) share the same secret.
  header: X-Hub-Signature-256
  how_to_obtain: Create a shared secret between the webhook sender and the function; the sender includes a hash of the payload in the designated header.
  location: header
  name: Webhook HMAC
  type: hmac
- evidence: The of-watchdog can protect a function with browser login through an OAuth 2.0 or OpenID Connect (OIDC) provider. It handles sign-in and checks the browser's session before forwarding requests to the function.
  how_to_obtain: Register the function as an OIDC client, configure oauth_enabled=true and provide client ID, issuer URL, and signing key; the watchdog performs the OAuth flow and sets a session cookie.
  location: cookie
  name: OAuth/OIDC login for functions
  type: oauth2
slug: openfaas-authentication
source_filename: openfaas-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.openfaas.com/reference/authentication/
source_yaml: "generated: '2026-10-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.openfaas.com/reference/authentication/\nsources:\n- https://docs.openfaas.com/reference/authentication/\n- https://docs.openfaas.com/reference/function-oauth/\ndescription: Authentication methods documented for OpenFaaS functions\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: You can also create and manage your own Bearer tokens or API keys. These are simply shared secrets, where the client (the user or\n    machine invoking the function) and the server (the function) share a copy of the token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token as a secret and assign it to the function; the client then sends it in the Authorization header.\n- type: http-basic\n  name: Basic authentication\n  evidence: 'You can enable basic-authentication for a web-portal or an API by setting the appropriate header such as WWW-Authenticate:\
  \ Basic\n    realm=\"User Visible Realm\" . This is the approach that the OpenFaaS gateway takes, and the OpenFaaS Pro edition comes with an OIDC integration.'\n  location: header\n  header: Authorization\n  how_to_obtain: Configure the gateway with a username and password; clients provide credentials using the HTTP Basic scheme.\n- type: hmac\n  name: Webhook HMAC\n  evidence: When functions receive webhooks, most publishers of events will not support any form of authentication. Messages are verified using\n    symmetric keys, where the client (your function) and the server (GitHub, Stripe, YouTube, etc) share the same secret.\n  location: header\n  header: X-Hub-Signature-256\n  how_to_obtain: Create a shared secret between the webhook sender and the function; the sender includes a hash of the payload in the designated\n    header.\n- type: oauth2\n  name: OAuth/OIDC login for functions\n  evidence: The of-watchdog can protect a function with browser login through an OAuth 2.0 or OpenID\
  \ Connect (OIDC) provider. It handles sign-in\n    and checks the browser's session before forwarding requests to the function.\n  location: cookie\n  how_to_obtain: Register the function as an OIDC client, configure oauth_enabled=true and provide client ID, issuer URL, and signing key; the\n    watchdog performs the OAuth flow and sets a session cookie.\ndocs: https://docs.openfaas.com/reference/authentication/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openfaas/refs/heads/main/authentication/openfaas-authentication.yml
summary_line: 4 schemes
tags:
- Company
- Serverless
- Open-source
- Functions
- Kubernetes
---
