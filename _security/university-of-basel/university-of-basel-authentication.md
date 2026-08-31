---
api_key_in: []
auth_types:
- none
- http_bearer
- openid_connect
- saml
description: 'The University of Basel issues no API keys and runs no developer credentialing of any kind. The one contract it serves — the UNIverse research information API — declares a bearer token and enforces it, but publishes no way for an outside developer to obtain one. Its open read surfaces — the edoc DSpace REST API and the edoc OAI-PMH interface — are open to anonymous callers with no token, no registration and no referer or origin check. Everything that IS authenticated at Basel is federated identity for people rather than credentials for machines: a SWITCHaai/eduGAIN SAML 2.0 identity provider scoped to unibas.ch, and an OpenID Connect issuer at sciCORE that brokers SWITCH edu-ID into research-computing services. Neither is a public API authorization server a third-party developer can register a client with; both are institutional single sign-on, readable from outside only through their published metadata.'
kind: authentication
layout: security
method: probed
name: University Of Basel Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Basel secures its APIs with none, http_bearer, openid_connect, and saml across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Basel
provider_slug: university-of-basel
scheme_count: 6
schemes:
- description: https://edoc.unibas.ch/server/api and its discovery, browse and metadata-registry endpoints answer HTTP 200 to an unauthenticated GET. Writes and the /server/api/authn endpoints require a Basel account; no self-service registration exists for outside developers.
  evidence:
    status: 200
    url: https://edoc.unibas.ch/server/api
  name: anonymous
  status: current
  surface: university-of-basel:edoc-rest
  type: none
- description: OAI-PMH is unauthenticated by protocol. Every verb — Identify, ListMetadataFormats, ListSets, ListRecords — answers anonymously.
  evidence:
    status: 200
    url: https://edoc.unibas.ch/server/oai/request?verb=Identify
  name: anonymous
  status: current
  surface: university-of-basel:edoc-oai
  type: none
- description: SAML 2.0 web browser SSO for people, federated through SWITCHaai and eduGAIN. Relying parties consume the IdP through the federation aggregate rather than through a per-service credential. The descriptor carries REFEDS Sirtfi assurance and REFEDS Research & Scholarship, so attribute release to R&S-tagged services is pre-agreed.
  evidence:
    status: 200
    url: https://metadata.aai.switch.ch/metadata.switchaai.xml
  name: saml2
  status: current
  surface: university-of-basel:switchaai-idp
  type: saml
- description: 'Keycloak realm switch-eduid at iam.scicore.unibas.ch. Discovery is public; client registration is not — no dynamic client registration endpoint is advertised, so a client must be created by sciCORE. Grant types advertised: authorization_code, client_credentials, implicit, password, refresh_token, device_code, jwt-bearer, token-exchange, uma-ticket and CIBA. Scopes advertised: openid, profile, email, phone, address, roles, organization, offline_access, service_account, basic, acr, web-origins, microprofile-jwt.'
  evidence:
    status: 200
    url: https://iam.scicore.unibas.ch/realms/switch-eduid/.well-known/openid-configuration
  name: openid-connect
  status: current
  surface: university-of-basel:scicore-oidc
  type: openid_connect
- description: 'The UNIverse research information API declares a single securityScheme named "Bearer Token". It is enforced: an anonymous GET of a data path returns HTTP 401 with {"timestamp":…,"status":401,"error":"Unauthorized","path":"/v2/publications"}. Tokens are issued to the university''s own applications; no registration or issuance flow is published.'
  evidence:
    status: 401
    url: https://universe-intern.unibas.ch/api/v2/publications
  name: bearer-token
  scheme: bearer
  status: current
  surface: university-of-basel:universe-research-information
  type: http
- description: ADAM's LTI launch endpoint validates a signed launch from a configured tool consumer. Without one it returns the ILIAS connection error. No public JWKS or tool-configuration document is served, so the LTI version could not be determined from outside.
  evidence:
    status: 200
    url: https://adam.unibas.ch/lti.php
  name: lti
  status: current
  surface: university-of-basel:adam-lti
  type: lti
slug: university-of-basel-authentication
source_filename: university-of-basel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live anonymous probes of every University of Basel institution-operated surface on 2026-08-30:\n  https://edoc.unibas.ch/server/api and /server/api/authn, the OAI-PMH interface at\n  /server/oai/request, the sciCORE OIDC discovery document at\n  https://iam.scicore.unibas.ch/realms/switch-eduid/.well-known/openid-configuration, the SWITCHaai\n  federation metadata for entityID https://aai-logon.unibas.ch/idp/shibboleth, and\n  https://adam.unibas.ch/lti.php.\nprovider: University of Basel\nproviderId: university-of-basel\nsummary:\n  types:\n  - none\n  - http_bearer\n  - openid_connect\n  - saml\n  oauth2: true\n  openid_connect: true\n  saml: true\n  mtls: false\n  api_keys: false\n  bearer_token: true\n  anonymous_read: true\ndescription: >-\n  The University of Basel issues no API keys and runs no developer credentialing of any kind. The\n  one contract it serves — the UNIverse research information API — declares a\
  \ bearer token and\n  enforces it, but publishes no way for an outside developer to obtain one. Its open\n  read surfaces — the edoc DSpace REST API and the edoc OAI-PMH interface — are open to anonymous\n  callers with no token, no registration and no referer or origin check. Everything that IS\n  authenticated at Basel is federated identity for people rather than credentials for machines:\n  a SWITCHaai/eduGAIN SAML 2.0 identity provider scoped to unibas.ch, and an OpenID Connect issuer\n  at sciCORE that brokers SWITCH edu-ID into research-computing services. Neither is a public API\n  authorization server a third-party developer can register a client with; both are institutional\n  single sign-on, readable from outside only through their published metadata.\nschemes:\n- name: anonymous\n  type: none\n  surface: university-of-basel:edoc-rest\n  status: current\n  description: >-\n    https://edoc.unibas.ch/server/api and its discovery, browse and metadata-registry endpoints\n    answer\
  \ HTTP 200 to an unauthenticated GET. Writes and the /server/api/authn endpoints require a\n    Basel account; no self-service registration exists for outside developers.\n  evidence:\n    url: https://edoc.unibas.ch/server/api\n    status: 200\n- name: anonymous\n  type: none\n  surface: university-of-basel:edoc-oai\n  status: current\n  description: >-\n    OAI-PMH is unauthenticated by protocol. Every verb — Identify, ListMetadataFormats, ListSets,\n    ListRecords — answers anonymously.\n  evidence:\n    url: https://edoc.unibas.ch/server/oai/request?verb=Identify\n    status: 200\n- name: saml2\n  type: saml\n  surface: university-of-basel:switchaai-idp\n  status: current\n  description: >-\n    SAML 2.0 web browser SSO for people, federated through SWITCHaai and eduGAIN. Relying parties\n    consume the IdP through the federation aggregate rather than through a per-service credential.\n    The descriptor carries REFEDS Sirtfi assurance and REFEDS Research & Scholarship, so attribute\n\
  \    release to R&S-tagged services is pre-agreed.\n  evidence:\n    url: https://metadata.aai.switch.ch/metadata.switchaai.xml\n    status: 200\n- name: openid-connect\n  type: openid_connect\n  surface: university-of-basel:scicore-oidc\n  status: current\n  description: >-\n    Keycloak realm switch-eduid at iam.scicore.unibas.ch. Discovery is public; client registration\n    is not — no dynamic client registration endpoint is advertised, so a client must be created by\n    sciCORE. Grant types advertised: authorization_code, client_credentials, implicit, password,\n    refresh_token, device_code, jwt-bearer, token-exchange, uma-ticket and CIBA. Scopes advertised:\n    openid, profile, email, phone, address, roles, organization, offline_access, service_account,\n    basic, acr, web-origins, microprofile-jwt.\n  evidence:\n    url: >-\n      https://iam.scicore.unibas.ch/realms/switch-eduid/.well-known/openid-configuration\n    status: 200\n- name: bearer-token\n  type: http\n  scheme:\
  \ bearer\n  surface: university-of-basel:universe-research-information\n  status: current\n  description: >-\n    The UNIverse research information API declares a single securityScheme named \"Bearer Token\".\n    It is enforced: an anonymous GET of a data path returns HTTP 401 with\n    {\"timestamp\":…,\"status\":401,\"error\":\"Unauthorized\",\"path\":\"/v2/publications\"}. Tokens are\n    issued to the university's own applications; no registration or issuance flow is published.\n  evidence:\n    url: https://universe-intern.unibas.ch/api/v2/publications\n    status: 401\n- name: lti\n  type: lti\n  surface: university-of-basel:adam-lti\n  status: current\n  description: >-\n    ADAM's LTI launch endpoint validates a signed launch from a configured tool consumer. Without\n    one it returns the ILIAS connection error. No public JWKS or tool-configuration document is\n    served, so the LTI version could not be determined from outside.\n  evidence:\n    url: https://adam.unibas.ch/lti.php\n\
  \    status: 200\nnotes: >-\n  No API key issuance, mTLS surface or signed-request scheme is published anywhere under\n  unibas.ch, and no authorization server accepts an outside client: the sciCORE Keycloak realm is\n  the only OAuth 2.0 / OIDC endpoint set on a Basel host and it advertises no dynamic client\n  registration. The bearer-JWT scheme previously recorded in this file belonged to DSP-API\n  (api.dasch.swiss), which is operated by DaSCH and was removed from this repository on\n  2026-08-30.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/authentication/university-of-basel-authentication.yml
summary_line: none/http_bearer/openid_connect/saml · 6 schemes
tags:
- University
- Higher Education
- Education
- Switzerland
- Basel
- Research Data
- Research Information
- Institutional Repository
- Open Access
- OAI-PMH
- Identity Federation
- Library
- Research Computing
---
