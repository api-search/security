---
api_key_in: []
auth_types:
- ws-federation
- openIdConnect
- oauth2
- session-cookie
description: ''
kind: authentication
layout: security
method: searched
name: Caa Insurance Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- deviceCode
overview: CAA Insurance secures its APIs with ws-federation, openIdConnect, oauth2, and session-cookie across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, and deviceCode flow(s).
provider_name: CAA Insurance
provider_slug: caa-insurance
scheme_count: 4
schemes:
- identity_provider: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/wsfed
  name: BrokerPortalFederation
  note: Observed on the redirect chain from http://www.caabrokerportal.ca/. The relying party is a SharePoint broker workspace; brokers, not developers, are the audience.
  relying_party: urn:sharepoint:federation
  surface: https://www.caabrokerportal.ca/
  type: ws-federation
- authorization_endpoint: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/authorize
  device_authorization_endpoint: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/devicecode
  end_session_endpoint: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/logout
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://018aba37-21fa-4b10-9382-01cdc448ba66.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/v2.0
  jwks_uri: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/discovery/v2.0/keys
  mtls_bound_access_tokens: true
  mtls_token_endpoint: https://mtlsauth.microsoft.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/token
  name: EntraExternalIdCIAM
  note: Anonymously served, standards-compliant OIDC discovery for the CAA Club Group CIAM tenant. Client registration is not open — there is no public developer app registration path, so these endpoints are documentation of the identity model, not an integration invitation.
  openIdConnectUrl: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/v2.0/.well-known/openid-configuration
  response_types_supported:
  - code
  - id_token
  - code id_token
  - id_token token
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  source: well-known/caa-insurance-openid-configuration.json
  subject_types_supported:
  - pairwise
  tenant_region_scope: NA
  token_endpoint: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - private_key_jwt
  - client_secret_basic
  - self_signed_tls_client_auth
  type: openIdConnect
  userinfo_endpoint: https://graph.microsoft.com/oidc/userinfo
- name: SharePointSoapSession
  note: Twenty SharePoint SOAP WSDL documents are served anonymously; every data operation requires an authenticated SharePoint session. The REST/OData sibling at /_api/web returns HTTP 403 System.UnauthorizedAccessException anonymously, and /_vti_bin/lists.asmx?WSDL returns 403.
  source: wsdl/_index.yml
  surface: https://www.caabrokerportal.ca/_vti_bin/*.asmx
  type: session
- name: CustomerPortalSession
  note: Next.js application login. Every route, including /.well-known/*, 307s to /sign-in?callbackUrl=... ; no anonymous OIDC or OAuth metadata is served.
  surface: https://customer.caainsurancecompany.ca/
  type: session
slug: caa-insurance-authentication
source_filename: caa-insurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  live probes 2026-07-25 of caabrokerportal.ca, customer.caainsurancecompany.ca\n  and the Microsoft Entra External ID (CIAM) tenant discovery document at\n  ccgexternalid.ciamlogin.com\nnote: >-\n  CAA Insurance publishes no API authentication documentation because it\n  publishes no API. This profile records the authentication surfaces that are\n  actually observable on CAA-operated hosts: a WS-Federation / OpenID Connect\n  identity provider fronting the broker portal, an application session login on\n  the customer portal, and an anonymous-WSDL / authenticated-operation SOAP\n  surface on the broker portal itself. No API key, bearer token, or mTLS client\n  contract is offered to third-party developers.\nsummary:\n  types: [ws-federation, openIdConnect, oauth2, session-cookie]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit, deviceCode]\n  developer_facing_credential: none\nschemes:\n- name: BrokerPortalFederation\n\
  \  type: ws-federation\n  surface: https://www.caabrokerportal.ca/\n  identity_provider: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/wsfed\n  relying_party: urn:sharepoint:federation\n  note: >-\n    Observed on the redirect chain from http://www.caabrokerportal.ca/. The\n    relying party is a SharePoint broker workspace; brokers, not developers, are\n    the audience.\n- name: EntraExternalIdCIAM\n  type: openIdConnect\n  openIdConnectUrl: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/v2.0/.well-known/openid-configuration\n  source: well-known/caa-insurance-openid-configuration.json\n  issuer: https://018aba37-21fa-4b10-9382-01cdc448ba66.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/v2.0\n  authorization_endpoint: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/authorize\n  token_endpoint: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/token\n  device_authorization_endpoint:\
  \ https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/devicecode\n  end_session_endpoint: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/logout\n  jwks_uri: https://ccgexternalid.ciamlogin.com/018aba37-21fa-4b10-9382-01cdc448ba66/discovery/v2.0/keys\n  userinfo_endpoint: https://graph.microsoft.com/oidc/userinfo\n  response_types_supported: [code, id_token, code id_token, id_token token]\n  token_endpoint_auth_methods_supported: [client_secret_post, private_key_jwt, client_secret_basic, self_signed_tls_client_auth]\n  id_token_signing_alg_values_supported: [RS256]\n  subject_types_supported: [pairwise]\n  scopes_supported: [openid, profile, email, offline_access]\n  mtls_bound_access_tokens: true\n  mtls_token_endpoint: https://mtlsauth.microsoft.com/018aba37-21fa-4b10-9382-01cdc448ba66/oauth2/v2.0/token\n  tenant_region_scope: NA\n  note: >-\n    Anonymously served, standards-compliant OIDC discovery for the CAA Club\n\
  \    Group CIAM tenant. Client registration is not open — there is no public\n    developer app registration path, so these endpoints are documentation of the\n    identity model, not an integration invitation.\n- name: SharePointSoapSession\n  type: session\n  surface: https://www.caabrokerportal.ca/_vti_bin/*.asmx\n  source: wsdl/_index.yml\n  note: >-\n    Twenty SharePoint SOAP WSDL documents are served anonymously; every data\n    operation requires an authenticated SharePoint session. The REST/OData\n    sibling at /_api/web returns HTTP 403 System.UnauthorizedAccessException\n    anonymously, and /_vti_bin/lists.asmx?WSDL returns 403.\n- name: CustomerPortalSession\n  type: session\n  surface: https://customer.caainsurancecompany.ca/\n  note: >-\n    Next.js application login. Every route, including /.well-known/*, 307s to\n    /sign-in?callbackUrl=... ; no anonymous OIDC or OAuth metadata is served.\npublic_api_auth:\n  available: false\n  note: >-\n    No API key programme, no\
  \ OAuth client registration, no developer\n    credentials of any kind are offered by CAA Insurance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caa-insurance/refs/heads/main/authentication/caa-insurance-authentication.yml
summary_line: ws-federation/openIdConnect/oauth2/session-cookie · 4 schemes
tags:
- Insurance
- Canada
- Property and Casualty
- Auto Insurance
- Home Insurance
- Carrier
- Brokers
- Personal Lines
- Telematics
- Partner Gated
- No Public API
---
