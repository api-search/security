---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication profile of the apinity marketplace gateway (the Kong-based engine that fronts every service sold on an apinity tenant, e.g. apinity Xplore). There is no OpenAPI for the gateway itself; this profile is read from the end-user documentation. Every request carries the CONSUMER CLIENT token obtained from a per-subscription /login endpoint; the upstream provider's own credential, when the provider chose pass-through authorization, travels in the ordinary Authorization header alongside it.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Apinity Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Apinity.io declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Apinity.io
provider_slug: apinity-io
scheme_count: 3
schemes:
- credential_issuance: API key generated when a Consumer Client of type API-Key is created in My Hub; shown once, cannot be retrieved later, can be regenerated
  docs: https://docs.apinity.io/step-by-step/subscribe-and-consume-a-service/consume-an-api-technical-implementation#consumeanapi-technicalimplementation-accessapiandauthenticationwithanapikey
  flow: 'POST {gateway_base}/login with JSON body {"api-key": "<key>"} (Content-Type: application/json). A 200 returns {"expires_in": <seconds>, "access_token": "Basic ..."}; send that value verbatim in the x-apx-authorization header on every subsequent call.'
  id: consumerClientApiKey
  in: header
  name: x-apx-authorization
  token_lifetime: 31536000 seconds (exactly one year); repeat login calls inside the window return the same token; ending the subscription invalidates it
  type: apiKey
- credential_issuance: Client ID + Client Secret generated when a Consumer Client of type OAuth2 is created; the secret is shown once and can be regenerated; the type cannot be changed after creation
  discovery: well-known/apinity-io-openid-configuration.json
  docs: https://docs.apinity.io/step-by-step/subscribe-and-consume-a-service/consume-an-api-technical-implementation#consumeanapi-technicalimplementation-accessapiandauthenticationwithoauth2
  flow: POST {gateway_base}/login as application/x-www-form-urlencoded with grant_type=client_credentials, client_id, client_secret. Returns access_token ("Bearer eyJ..."), refresh_token, expires_in (300 in the docs' example) and refresh_token_expires_in (1800). Refresh with grant_type=refresh_token to the same endpoint. The access token is sent in the x-apx-authorization header.
  flows:
    clientCredentials:
      refreshUrl: https://api.marketplace.apinity.io/{EndpointURI}/login
      scopes: {}
      tokenUrl: https://api.marketplace.apinity.io/{EndpointURI}/login
  id: consumerClientOAuth2
  issuer: https://auth.apinity.io/realms/syncier-marketplace-engine
  scopes_note: no API scopes are documented; the example JWT carries the OIDC default scope "profile email" and is issued by the Keycloak realm below
  type: oauth2
- description: Optional second credential. When a service provider did not configure an Access Control on the gateway, subscribers send the provider's own credential in the Authorization header; the gateway forwards the request unmodified. When an Access Control IS configured, the gateway strips/replaces the Authorization header with the provider-side credential it holds (Basic, API-key header, username/password header, OAuth2 password or client-credentials, HMAC, auth-key header, JSON payload).
  docs: https://docs.apinity.io/concepts/authorization#2b.-pass-through-authorization
  id: providerPassThrough
  in: header
  name: Authorization
  scheme: provider-defined
  type: http
slug: apinity-io-authentication
source_filename: apinity-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: https://docs.apinity.io/step-by-step/subscribe-and-consume-a-service/consume-an-api-technical-implementation\ndocs:\n  - https://docs.apinity.io/concepts/authorization\n  - https://docs.apinity.io/step-by-step/subscribe-and-consume-a-service/consumer-clients\n  - https://docs.apinity.io/step-by-step/provide-a-service-on-the-marketplace/add-an-api\nprovider: Apinity.io\nproviderId: apinity-io\ndescription: >-\n  Authentication profile of the apinity marketplace gateway (the Kong-based engine that fronts every\n  service sold on an apinity tenant, e.g. apinity Xplore). There is no OpenAPI for the gateway itself;\n  this profile is read from the end-user documentation. Every request carries the CONSUMER CLIENT\n  token obtained from a per-subscription /login endpoint; the upstream provider's own credential, when\n  the provider chose pass-through authorization, travels in the ordinary Authorization header alongside it.\ngateway_base:\
  \ https://api.marketplace.apinity.io/{EndpointURI}\ngateway_base_note: >-\n  {EndpointURI} is unique per subscription and shown under Subscriptions > Technical Setup in the portal\n  (the docs' example is hello-world/639041ec-a6ba-4684-b37e-10677d482eb7). Probed 2026-09-18 the host\n  presents a *.apinity.io certificate that does not cover this two-level subdomain, so the documented\n  base cannot be reached over verified TLS; no live probe of the login flow was possible.\nschemes:\n  - id: consumerClientApiKey\n    type: apiKey\n    in: header\n    name: x-apx-authorization\n    flow: >-\n      POST {gateway_base}/login with JSON body {\"api-key\": \"<key>\"} (Content-Type: application/json).\n      A 200 returns {\"expires_in\": <seconds>, \"access_token\": \"Basic ...\"}; send that value verbatim in the\n      x-apx-authorization header on every subsequent call.\n    token_lifetime: 31536000 seconds (exactly one year); repeat login calls inside the window return the same token; ending\
  \ the subscription invalidates it\n    credential_issuance: API key generated when a Consumer Client of type API-Key is created in My Hub; shown once, cannot be retrieved later, can be regenerated\n    docs: https://docs.apinity.io/step-by-step/subscribe-and-consume-a-service/consume-an-api-technical-implementation#consumeanapi-technicalimplementation-accessapiandauthenticationwithanapikey\n  - id: consumerClientOAuth2\n    type: oauth2\n    flows:\n      clientCredentials:\n        tokenUrl: https://api.marketplace.apinity.io/{EndpointURI}/login\n        refreshUrl: https://api.marketplace.apinity.io/{EndpointURI}/login\n        scopes: {}\n    flow: >-\n      POST {gateway_base}/login as application/x-www-form-urlencoded with grant_type=client_credentials,\n      client_id, client_secret. Returns access_token (\"Bearer eyJ...\"), refresh_token, expires_in (300 in the\n      docs' example) and refresh_token_expires_in (1800). Refresh with grant_type=refresh_token to the same\n      endpoint.\
  \ The access token is sent in the x-apx-authorization header.\n    scopes_note: no API scopes are documented; the example JWT carries the OIDC default scope \"profile email\" and is issued by the Keycloak realm below\n    issuer: https://auth.apinity.io/realms/syncier-marketplace-engine\n    discovery: well-known/apinity-io-openid-configuration.json\n    credential_issuance: Client ID + Client Secret generated when a Consumer Client of type OAuth2 is created; the secret is shown once and can be regenerated; the type cannot be changed after creation\n    docs: https://docs.apinity.io/step-by-step/subscribe-and-consume-a-service/consume-an-api-technical-implementation#consumeanapi-technicalimplementation-accessapiandauthenticationwithoauth2\n  - id: providerPassThrough\n    type: http\n    scheme: provider-defined\n    in: header\n    name: Authorization\n    description: >-\n      Optional second credential. When a service provider did not configure an Access Control on the\n      gateway,\
  \ subscribers send the provider's own credential in the Authorization header; the gateway\n      forwards the request unmodified. When an Access Control IS configured, the gateway strips/replaces\n      the Authorization header with the provider-side credential it holds (Basic, API-key header,\n      username/password header, OAuth2 password or client-credentials, HMAC, auth-key header, JSON payload).\n    docs: https://docs.apinity.io/concepts/authorization#2b.-pass-through-authorization\nheader_notes:\n  - The consumer token may be sent in Authorization instead of x-apx-authorization only when the provider does not need Authorization for pass-through; the gateway consumes it either way.\n  - Since the October 2023 release x-apx-authorization is the canonical header; pre-existing subscriptions that send the gateway token in Authorization keep working.\nfailure_modes:\n  - status: 401\n    when: x-apx-authorization header absent — the gateway rejects before forwarding upstream\n  - status:\
  \ 403\n    when: header present but the token is invalid — also rejected at the gateway\n  - status: 404\n    when: the request URL omits the https:// prefix\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apinity-io/refs/heads/main/authentication/apinity-io-authentication.yml
summary_line: 3 schemes
tags:
- API Governance
- API Marketplace
- Compliance
- Discovery
- Integration Platform
---
