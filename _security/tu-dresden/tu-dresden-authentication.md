---
api_key_in: []
auth_types: []
description: 'How the TU Dresden surfaces recorded in apis.yml are authenticated, established by probing each one from outside the institution''s network on 2026-08-30. Every scheme below was observed in a live response or read from TU Dresden''s own documentation — none is inferred from an OpenAPI, because TU Dresden publishes no OpenAPI of its own. TU Dresden issues no self-service developer credential to the general public: every credential here is bound to an institutional affiliation, which is the normal shape for a university and is recorded rather than treated as a gap.'
kind: authentication
layout: security
method: probed
name: Tu Dresden Authentication
name_suffix: Authentication
oauth_flows: []
overview: TU Dresden declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: TU Dresden
provider_slug: tu-dresden
scheme_count: 5
schemes:
- evidence: 'GET https://llm.scads.ai/v1/models with no credential returns HTTP 500 with {"error":{"message":"No api key passed in.","type":"auth_error","param":"None","code":"500"}}. The same request bearing Authorization: Bearer sk-not-a-real-key returns a DIFFERENT body — "Authentication Error, Invalid proxy server token passed. Received API Key = sk-...-key, Key Hash (Token) =d748053a…, Unable to find token in cache or `LiteLLM_VerificationTokenTable`" — which proves the token is validated against a store rather than merely required. The documented base URL is https://llm.scads.ai/v1 and the service is OpenAI-compatible, so any official OpenAI client authenticates by pointing at that base URL.'
  format: Bearer <TUD:AI API key>
  header: Authorization
  id: tud-ai-bearer
  in: header
  issuance: TU Dresden employees generate a key themselves at https://selfservice.tu-dresden.de/services/scads-llm-api/ (the institution's Self-Service Portal, which itself requires a TU Dresden account). Students and ScaDS.AI-affiliated externals request one by email to llm.scads.ai@tu-dresden.de. There is no public signup.
  onboarding: affiliation
  quotas: TU Dresden's documentation states that keys created through the Self-Service Portal carry a restrictive requests-per-minute limit by default, with higher limits available on request. The numeric limit is not published.
  scheme: bearer
  surface: tu-dresden:tud-ai-llm
  type: apiKey
- evidence: GET https://vvz.phil.tu-dresden.de/api?auth_code=test returns HTTP 200 with the plain-text body "Der Auth-Code ist leider nicht richtig." — the code is checked, and a wrong one is rejected in German with a 200 status rather than a 401. GET https://vvz.phil.tu-dresden.de/api with no parameter returns the human documentation page.
  id: vvz-auth-code
  in: query
  issuance: An API account is issued on request through the lecture directory's contact page; the documentation states that anyone interested can ask for one. The account yields an auth_code appended to every request.
  onboarding: request
  parameter: auth_code
  quotas: The documentation requires at least ten seconds between calls. No numeric quota is published and no 429 was observed.
  surface: tu-dresden:lecture-catalog
  type: apiKey
- evidence: GET https://opara.zih.tu-dresden.de/server/api returns HTTP 200 anonymously with the DSpace HAL root document (dspaceName "OPARA Research Data Repository", dspaceVersion "DSpace 7.6.2") listing an authn link. GET /server/api/core/collections and /server/api/discover/search/objects both return 200 with live data and no credential.
  id: opara-open-read
  issuance: Read access to public communities, collections, items and bitstreams needs no credential. Deposit, workflow and administrative operations authenticate through the DSpace 7 authentication endpoint at https://opara.zih.tu-dresden.de/server/api/authn, which for TU Dresden members is backed by the institution's Shibboleth identity provider.
  onboarding: none
  surface: tu-dresden:opara-rest
  type: none
- evidence: https://idp.tu-dresden.de/idp/shibboleth serves signed SAML 2.0 metadata registered by https://www.aai.dfn.de. https://idp.tu-dresden.de/.well-known/openid-configuration returns issuer https://idp.tu-dresden.de, response_types_supported [code], grant_types_supported [authorization_code], scopes_supported [openid], and token_endpoint_auth_methods_supported [client_secret_basic, client_secret_post, client_secret_jwt, private_key_jwt]. https://idp.tu-dresden.de/idp/profile/oidc/keyset serves a three-key JWKS.
  id: idp-saml-oidc
  issuance: Service providers do not receive a credential from TU Dresden directly; they join DFN-AAI (or reach the entity through eduGAIN) and consume the published metadata. OIDC relying parties authenticate at the token endpoint with client_secret_basic, client_secret_post, client_secret_jwt or private_key_jwt.
  onboarding: federation
  protocols:
  - SAML 2.0 Web Browser SSO
  - SAML 2.0 ECP (SOAP, port 8443)
  - OpenID Connect authorization_code
  surface: tu-dresden:sso-shibboleth
  type: federated
- evidence: https://fis.tu-dresden.de/ws/api returns HTTP 403 from Apache with the server's generic Forbidden page — an edge denial, not an application auth challenge. /ws/oai?verb=Identify and /ws/rest return the same 403. /portal/ws/api returns 404. The public portal at https://fis.tu-dresden.de/portal/ answers 200 and identifies itself as Pure via a PureFacade marker in the page.
  id: pure-ws-key
  issuance: Elsevier Pure's web service is normally keyed per client by the institution's Pure administrators. TU Dresden publishes no request process, and the endpoint is not reachable from the public internet.
  onboarding: unknown
  operator: tenant
  surface: tu-dresden:fis-pure
  type: apiKey
slug: tu-dresden-authentication
source_filename: tu-dresden-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource:\n- https://llm.scads.ai/v1/models\n- https://llm.scads.ai/docs/usage/api/\n- https://selfservice.tu-dresden.de/services/scads-llm-api/\n- https://vvz.phil.tu-dresden.de/api\n- https://vvz.phil.tu-dresden.de/api?auth_code=test\n- https://opara.zih.tu-dresden.de/server/api\n- https://opara.zih.tu-dresden.de/server/api/authn\n- https://idp.tu-dresden.de/idp/shibboleth\n- https://idp.tu-dresden.de/.well-known/openid-configuration\n- https://fis.tu-dresden.de/ws/api\ndescription: >-\n  How the TU Dresden surfaces recorded in apis.yml are authenticated, established by probing each\n  one from outside the institution's network on 2026-08-30. Every scheme below was observed in a\n  live response or read from TU Dresden's own documentation — none is inferred from an OpenAPI,\n  because TU Dresden publishes no OpenAPI of its own. TU Dresden issues no self-service developer\n  credential to the general public: every credential here is bound\
  \ to an institutional\n  affiliation, which is the normal shape for a university and is recorded rather than treated as\n  a gap.\nschemes:\n- id: tud-ai-bearer\n  surface: tu-dresden:tud-ai-llm\n  type: apiKey\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <TUD:AI API key>'\n  onboarding: affiliation\n  issuance: >-\n    TU Dresden employees generate a key themselves at\n    https://selfservice.tu-dresden.de/services/scads-llm-api/ (the institution's Self-Service\n    Portal, which itself requires a TU Dresden account). Students and ScaDS.AI-affiliated\n    externals request one by email to llm.scads.ai@tu-dresden.de. There is no public signup.\n  evidence: >-\n    GET https://llm.scads.ai/v1/models with no credential returns HTTP 500 with\n    {\"error\":{\"message\":\"No api key passed in.\",\"type\":\"auth_error\",\"param\":\"None\",\"code\":\"500\"}}.\n    The same request bearing Authorization: Bearer sk-not-a-real-key returns a DIFFERENT body —\n   \
  \ \"Authentication Error, Invalid proxy server token passed. Received API Key = sk-...-key, Key\n    Hash (Token) =d748053a…, Unable to find token in cache or `LiteLLM_VerificationTokenTable`\" —\n    which proves the token is validated against a store rather than merely required. The\n    documented base URL is https://llm.scads.ai/v1 and the service is OpenAI-compatible, so any\n    official OpenAI client authenticates by pointing at that base URL.\n  quotas: >-\n    TU Dresden's documentation states that keys created through the Self-Service Portal carry a\n    restrictive requests-per-minute limit by default, with higher limits available on request.\n    The numeric limit is not published.\n- id: vvz-auth-code\n  surface: tu-dresden:lecture-catalog\n  type: apiKey\n  in: query\n  parameter: auth_code\n  onboarding: request\n  issuance: >-\n    An API account is issued on request through the lecture directory's contact page; the\n    documentation states that anyone interested can ask\
  \ for one. The account yields an auth_code\n    appended to every request.\n  evidence: >-\n    GET https://vvz.phil.tu-dresden.de/api?auth_code=test returns HTTP 200 with the plain-text\n    body \"Der Auth-Code ist leider nicht richtig.\" — the code is checked, and a wrong one is\n    rejected in German with a 200 status rather than a 401. GET\n    https://vvz.phil.tu-dresden.de/api with no parameter returns the human documentation page.\n  quotas: >-\n    The documentation requires at least ten seconds between calls. No numeric quota is published\n    and no 429 was observed.\n- id: opara-open-read\n  surface: tu-dresden:opara-rest\n  type: none\n  onboarding: none\n  issuance: >-\n    Read access to public communities, collections, items and bitstreams needs no credential.\n    Deposit, workflow and administrative operations authenticate through the DSpace 7\n    authentication endpoint at https://opara.zih.tu-dresden.de/server/api/authn, which for TU\n    Dresden members is backed\
  \ by the institution's Shibboleth identity provider.\n  evidence: >-\n    GET https://opara.zih.tu-dresden.de/server/api returns HTTP 200 anonymously with the DSpace\n    HAL root document (dspaceName \"OPARA Research Data Repository\", dspaceVersion \"DSpace 7.6.2\")\n    listing an authn link. GET /server/api/core/collections and\n    /server/api/discover/search/objects both return 200 with live data and no credential.\n- id: idp-saml-oidc\n  surface: tu-dresden:sso-shibboleth\n  type: federated\n  protocols:\n  - SAML 2.0 Web Browser SSO\n  - SAML 2.0 ECP (SOAP, port 8443)\n  - OpenID Connect authorization_code\n  onboarding: federation\n  issuance: >-\n    Service providers do not receive a credential from TU Dresden directly; they join DFN-AAI (or\n    reach the entity through eduGAIN) and consume the published metadata. OIDC relying parties\n    authenticate at the token endpoint with client_secret_basic, client_secret_post,\n    client_secret_jwt or private_key_jwt.\n  evidence:\
  \ >-\n    https://idp.tu-dresden.de/idp/shibboleth serves signed SAML 2.0 metadata registered by\n    https://www.aai.dfn.de. https://idp.tu-dresden.de/.well-known/openid-configuration returns\n    issuer https://idp.tu-dresden.de, response_types_supported [code], grant_types_supported\n    [authorization_code], scopes_supported [openid], and\n    token_endpoint_auth_methods_supported [client_secret_basic, client_secret_post,\n    client_secret_jwt, private_key_jwt]. https://idp.tu-dresden.de/idp/profile/oidc/keyset serves\n    a three-key JWKS.\n- id: pure-ws-key\n  surface: tu-dresden:fis-pure\n  type: apiKey\n  onboarding: unknown\n  operator: tenant\n  issuance: >-\n    Elsevier Pure's web service is normally keyed per client by the institution's Pure\n    administrators. TU Dresden publishes no request process, and the endpoint is not reachable\n    from the public internet.\n  evidence: >-\n    https://fis.tu-dresden.de/ws/api returns HTTP 403 from Apache with the server's generic\n\
  \    Forbidden page — an edge denial, not an application auth challenge. /ws/oai?verb=Identify and\n    /ws/rest return the same 403. /portal/ws/api returns 404. The public portal at\n    https://fis.tu-dresden.de/portal/ answers 200 and identifies itself as Pure via a PureFacade\n    marker in the page.\nnotes: >-\n  No OAuth 2.0 authorization server, no client-credentials flow and no developer key management\n  console exists on any TU Dresden host outside the identity provider itself. The institution\n  publishes a security.txt at https://tu-dresden.de/.well-known/security.txt naming\n  cert@tu-dresden.de, which is recorded separately under security/.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tu-dresden/refs/heads/main/authentication/tu-dresden-authentication.yml
summary_line: 5 schemes
tags:
- University
- Higher Education
- Education
- Germany
- Saxony
- TU9
- Research
- Research Data
- Research Computing
- Artificial Intelligence
- Identity Federation
- OAI-PMH
- Institutional Repository
- Open Access
---
