---
api_key_in:
- header
- basic-username
auth_types:
- none
- http
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Ieso Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refreshToken
- password
- deviceCode
overview: IESO secures its APIs with none, http, apiKey, oauth2, and openIdConnect across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, refreshToken, password, and deviceCode flow(s).
provider_name: IESO
provider_slug: ieso
scheme_count: 6
schemes:
- applies_to: ieso:ieso-public-reports-repository
  description: No authentication of any kind. IMO_SPEC_0100 section 3 states "All market participants, and in general, the public, have access to public report repository." Verified HTTP 200 anonymously on 2026-07-27 on both the directory index and a live data file. No account, key, cookie, referrer check or terms click-through.
  evidence: https://www.ieso.ca/-/media/Files/IESO/technical-interfaces/xml-automated-docs/IMO_SPEC_0100.pdf
  hosts:
  - https://reports-public.ieso.ca
  - https://reports-public-sandbox.ieso.ca
  name: public-report-repository-anonymous
  type: none
- applies_to: ieso:ieso-reports-site-rest-api
  description: HTTP Basic credentials on every request to the Axway SecureTransport REST API, plus the mandatory query string parameter ?idp_id=ieso appended to every request. The IESO Reports API Guide states "The market participant must have a valid user name and password in order to access the confidential report repository (upon request the IESO shall provide the market participant with a machine account)."
  evidence: https://www.ieso.ca/-/media/Files/IESO/technical-interfaces/api-reports-guide/IESO_Reports_API_Guide.pdf
  hosts:
  - https://reports.ieso.ca
  - https://reports-sandbox.ieso.ca
  name: reports-api-basic
  probe:
    date: '2026-07-27'
    status: 401
    url: https://reports.ieso.ca/api/v1.4/files?idp_id=ieso
  required_query_parameter: idp_id=ieso
  scheme: basic
  type: http
- applies_to: ieso:ieso-reports-site-rest-api
  description: A second access interface to the same confidential repository. SSH File Transfer Protocol on port 22 with the same machine API account username and password. Documented in the IESO Reports API Guide, "Access Interface - SFTP".
  evidence: https://www.ieso.ca/-/media/Files/IESO/technical-interfaces/api-reports-guide/IESO_Reports_API_Guide.pdf
  hosts:
  - reports.ieso.ca:22
  name: reports-sftp
  scheme: sftp-password
  type: http
- applies_to:
  - ieso:ieso-registration-facilities-api
  - ieso:ieso-retrofit-api
  - ieso:ieso-retrofit-service-provider-api
  description: 'Appian API key, accepted three ways per SPEC-249: HTTP Basic with the API key as the username and a blank password (or the reverse), an Appian-API-Key request header, or an Authorization Bearer header. HTTPS is mandatory. A missing or invalid Authorization header returns 401.'
  evidence: https://www.ieso.ca/-/media/Files/IESO/technical-interfaces/registration-system/FacilityAPISpecification-SPEC-249.pdf
  hosts:
  - https://online.ieso.ca
  - https://onlinesandbox.ieso.ca
  in:
  - header
  - basic-username
  issuance: The organization's registered IESO Rights Administrator must request an API machine account with "Registration API" access. No self-serve issuance.
  name: appian-api-key
  parameter_names:
  - Appian-API-Key
  - Authorization
  type: apiKey
- applies_to: ieso:ieso-mim-web-services
  description: SOAP endpoint secured by an IESO UserID and password in the format user@participantName, combined with source IP address allow-listing and a client truststore. IESO's technical interfaces page states the MIM web services require "UserID/Password and whitelisted client machine IP address". Neither the production nor sandbox host connected from the open internet on 2026-07-27 (curl exit 000), consistent with network-level restriction.
  evidence: https://www.ieso.ca/-/media/Files/IESO/technical-interfaces/mp-submissions/MWT-User-Guide.pdf
  hosts:
  - https://webservices.ieso.ca
  - https://webservices-sandbox.ieso.ca
  - https://webservices-sandboxmrp.ieso.ca
  name: mim-userid-password-plus-ip-allowlist
  scheme: ws-security-userid-password
  transport_controls:
  - ip-allowlist
  - client-truststore
  - tls
  type: http
  username_format: user@participantName
- applies_to: participant web applications (reports.ieso.ca, online.ieso.ca)
  authorization_endpoint: https://gateway.ieso.ca/oauth2/v1/authorize
  code_challenge_methods_supported:
  - S256
  description: The Okta-hosted identity provider that fronts interactive participant login. reports.ieso.ca auto-POSTs a SAML2 AuthnRequest to this gateway. The OIDC/OAuth 2.0 discovery documents are served anonymously and are harvested to well-known/. This is the human login path, not the machine-account path used by the documented APIs.
  device_authorization_endpoint: https://gateway.ieso.ca/oauth2/v1/device/authorize
  dpop_supported: true
  grant_types_supported:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - urn:ietf:params:oauth:grant-type:device_code
  introspection_endpoint: https://gateway.ieso.ca/oauth2/v1/introspect
  issuer: https://gateway.ieso.ca
  jwks_uri: https://gateway.ieso.ca/oauth2/v1/keys
  name: ieso-gateway-oidc
  openIdConnectUrl: https://gateway.ieso.ca/.well-known/openid-configuration
  registration_endpoint: https://gateway.ieso.ca/oauth2/v1/clients
  revocation_endpoint: https://gateway.ieso.ca/oauth2/v1/revoke
  source: well-known/ieso-openid-configuration.json
  token_endpoint: https://gateway.ieso.ca/oauth2/v1/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  - client_secret_jwt
  - private_key_jwt
  - none
  type: openIdConnect
  userinfo_endpoint: https://gateway.ieso.ca/oauth2/v1/userinfo
slug: ieso-authentication
source_filename: ieso-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  IESO published interface specifications (IMO_SPEC_0100, IESO_Reports_API_Guide, SPEC-249, SPEC-188,\n  MWT-User-Guide) plus anonymous probes of every host and the live OIDC discovery document at\n  gateway.ieso.ca\ndocs: https://www.ieso.ca/sector-participants/technical-interfaces\nnote: >-\n  Derived mechanically from OpenAPI is not possible here — IESO publishes no OpenAPI. This profile is\n  read from IESO's own published interface specifications and confirmed by live probes. The estate has\n  four distinct authentication models and one genuinely unauthenticated surface.\nsummary:\n  types: [none, http, apiKey, oauth2, openIdConnect]\n  api_key_in: [header, basic-username]\n  oauth2_flows: [authorizationCode, implicit, refreshToken, password, deviceCode]\n  anonymous_surfaces: 1\n  self_serve_credentials: false\n  credential_issuance: >-\n    No self-serve signup for any authenticated surface. Machine accounts and\
  \ API keys are issued by\n    the IESO on request, and for the Online IESO APIs must be requested by the participant\n    organization's registered Rights Administrator.\nschemes:\n- name: public-report-repository-anonymous\n  type: none\n  applies_to: ieso:ieso-public-reports-repository\n  hosts: [https://reports-public.ieso.ca, https://reports-public-sandbox.ieso.ca]\n  description: >-\n    No authentication of any kind. IMO_SPEC_0100 section 3 states \"All market participants, and in\n    general, the public, have access to public report repository.\" Verified HTTP 200 anonymously on\n    2026-07-27 on both the directory index and a live data file. No account, key, cookie, referrer\n    check or terms click-through.\n  evidence: https://www.ieso.ca/-/media/Files/IESO/technical-interfaces/xml-automated-docs/IMO_SPEC_0100.pdf\n- name: reports-api-basic\n  type: http\n  scheme: basic\n  applies_to: ieso:ieso-reports-site-rest-api\n  hosts: [https://reports.ieso.ca, https://reports-sandbox.ieso.ca]\n\
  \  description: >-\n    HTTP Basic credentials on every request to the Axway SecureTransport REST API, plus the mandatory\n    query string parameter ?idp_id=ieso appended to every request. The IESO Reports API Guide states\n    \"The market participant must have a valid user name and password in order to access the\n    confidential report repository (upon request the IESO shall provide the market participant with a\n    machine account).\"\n  required_query_parameter: idp_id=ieso\n  probe:\n    url: https://reports.ieso.ca/api/v1.4/files?idp_id=ieso\n    status: 401\n    date: '2026-07-27'\n  evidence: https://www.ieso.ca/-/media/Files/IESO/technical-interfaces/api-reports-guide/IESO_Reports_API_Guide.pdf\n- name: reports-sftp\n  type: http\n  scheme: sftp-password\n  applies_to: ieso:ieso-reports-site-rest-api\n  hosts: [reports.ieso.ca:22]\n  description: >-\n    A second access interface to the same confidential repository. SSH File Transfer Protocol on port\n    22 with the same\
  \ machine API account username and password. Documented in the IESO Reports API\n    Guide, \"Access Interface - SFTP\".\n  evidence: https://www.ieso.ca/-/media/Files/IESO/technical-interfaces/api-reports-guide/IESO_Reports_API_Guide.pdf\n- name: appian-api-key\n  type: apiKey\n  applies_to:\n  - ieso:ieso-registration-facilities-api\n  - ieso:ieso-retrofit-api\n  - ieso:ieso-retrofit-service-provider-api\n  hosts: [https://online.ieso.ca, https://onlinesandbox.ieso.ca]\n  description: >-\n    Appian API key, accepted three ways per SPEC-249: HTTP Basic with the API key as the username and\n    a blank password (or the reverse), an Appian-API-Key request header, or an Authorization Bearer\n    header. HTTPS is mandatory. A missing or invalid Authorization header returns 401.\n  in: [header, basic-username]\n  parameter_names: [Appian-API-Key, Authorization]\n  issuance: >-\n    The organization's registered IESO Rights Administrator must request an API machine account with\n    \"Registration\
  \ API\" access. No self-serve issuance.\n  evidence: https://www.ieso.ca/-/media/Files/IESO/technical-interfaces/registration-system/FacilityAPISpecification-SPEC-249.pdf\n- name: mim-userid-password-plus-ip-allowlist\n  type: http\n  scheme: ws-security-userid-password\n  applies_to: ieso:ieso-mim-web-services\n  hosts: [https://webservices.ieso.ca, https://webservices-sandbox.ieso.ca, https://webservices-sandboxmrp.ieso.ca]\n  description: >-\n    SOAP endpoint secured by an IESO UserID and password in the format user@participantName, combined\n    with source IP address allow-listing and a client truststore. IESO's technical interfaces page\n    states the MIM web services require \"UserID/Password and whitelisted client machine IP address\".\n    Neither the production nor sandbox host connected from the open internet on 2026-07-27 (curl exit\n    000), consistent with network-level restriction.\n  username_format: user@participantName\n  transport_controls: [ip-allowlist, client-truststore,\
  \ tls]\n  evidence: https://www.ieso.ca/-/media/Files/IESO/technical-interfaces/mp-submissions/MWT-User-Guide.pdf\n- name: ieso-gateway-oidc\n  type: openIdConnect\n  applies_to: participant web applications (reports.ieso.ca, online.ieso.ca)\n  openIdConnectUrl: https://gateway.ieso.ca/.well-known/openid-configuration\n  issuer: https://gateway.ieso.ca\n  description: >-\n    The Okta-hosted identity provider that fronts interactive participant login. reports.ieso.ca\n    auto-POSTs a SAML2 AuthnRequest to this gateway. The OIDC/OAuth 2.0 discovery documents are served\n    anonymously and are harvested to well-known/. This is the human login path, not the machine-account\n    path used by the documented APIs.\n  authorization_endpoint: https://gateway.ieso.ca/oauth2/v1/authorize\n  token_endpoint: https://gateway.ieso.ca/oauth2/v1/token\n  userinfo_endpoint: https://gateway.ieso.ca/oauth2/v1/userinfo\n  jwks_uri: https://gateway.ieso.ca/oauth2/v1/keys\n  introspection_endpoint: https://gateway.ieso.ca/oauth2/v1/introspect\n\
  \  revocation_endpoint: https://gateway.ieso.ca/oauth2/v1/revoke\n  device_authorization_endpoint: https://gateway.ieso.ca/oauth2/v1/device/authorize\n  registration_endpoint: https://gateway.ieso.ca/oauth2/v1/clients\n  grant_types_supported: [authorization_code, implicit, refresh_token, password, 'urn:ietf:params:oauth:grant-type:device_code']\n  token_endpoint_auth_methods_supported: [client_secret_basic, client_secret_post, client_secret_jwt, private_key_jwt, none]\n  code_challenge_methods_supported: [S256]\n  dpop_supported: true\n  source: well-known/ieso-openid-configuration.json\ngaps:\n- No API key or token can be obtained self-serve anywhere in the estate.\n- No mTLS scheme is documented for any interface.\n- >-\n  The scopes advertised by gateway.ieso.ca are the stock OIDC set; IESO publishes no\n  API-specific authorization scope catalogue. See scopes/ieso-scopes.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ieso/refs/heads/main/authentication/ieso-authentication.yml
summary_line: none/http/apiKey/oauth2/openIdConnect · 6 schemes
tags:
- Energy
- Canada
- Electricity
- Energy Markets
- Grid
- System Operator
- Market Data
- Open Data
- Ontario
- Demand Response
- Renewables
---
