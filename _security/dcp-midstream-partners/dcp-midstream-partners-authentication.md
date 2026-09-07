---
anonymous_access: false
api_key_in: []
auth_types:
- openIdConnect
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Dcp Midstream Partners Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: DCP Midstream Partners secures its APIs with openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: DCP Midstream Partners
provider_slug: dcp-midstream-partners
scheme_count: 2
schemes:
- application: https://fits.ephillips66.com/
  claims_supported:
  - email
  - sub
  - tid
  - given_name
  - family_name
  - name
  - businessPhone
  - companyName
  - newUser
  - termsOfUseVersionAccepted
  end_session_endpoint: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/b2c_1a_fits_signupsignin/oauth2/logout
  flows:
  - authorizationUrl: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/b2c_1a_fits_signupsignin/oauth2/authorize
    flow: authorizationCode
    pkce: S256
    tokenUrl: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/b2c_1a_fits_signupsignin/oauth2/token
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://azrmdstadb2cr5.b2clogin.com/e1fdebb4-638c-48e6-b771-2413e270655c/v2.0/
  jwks_uri: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/b2c_1a_fits_signupsignin/discovery/keys
  name: fits-b2c
  openIdConnectUrl: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/B2C_1A_FITS_SIGNUPSIGNIN/v2.0/.well-known/openid-configuration
  policy: B2C_1A_FITS_SIGNUPSIGNIN
  provider: Azure AD B2C
  scopes_supported:
  - openid
  sources:
  - well-known/dcp-midstream-partners-fits-openid-configuration.json
  subject_types_supported:
  - pairwise
  system: FITS (Field Information & Technology Services)
  type: openIdConnect
- application: https://alnlogin.ephillips66.com/
  claims_supported:
  - SubjectNamingInfo
  - objectId
  - businessPhone
  - companyName
  - newUser
  - termsOfUseVersionAccepted
  flows:
  - authorizationUrl: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/b2c_1a_aligneapp_signupsignin/oauth2/authorize
    flow: authorizationCode
    tokenUrl: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/b2c_1a_aligneapp_signupsignin/oauth2/token
  issuer: https://azrmdstadb2cr5.b2clogin.com/e1fdebb4-638c-48e6-b771-2413e270655c/v2.0/
  name: aligne-b2c
  openIdConnectUrl: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/B2C_1A_ALIGNEAPP_SIGNUPSIGNIN/v2.0/.well-known/openid-configuration
  policy: B2C_1A_ALIGNEAPP_SIGNUPSIGNIN
  provider: Azure AD B2C
  relying_party: https://azrmdstadb2cr5.onmicrosoft.com/AligneApp
  scopes_supported:
  - openid
  sources:
  - well-known/dcp-midstream-partners-aligne-openid-configuration.json
  system: Aligne — natural gas scheduling, customer activities & informational postings
  type: openIdConnect
slug: dcp-midstream-partners-authentication
source_filename: dcp-midstream-partners-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: >-\n  https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/B2C_1A_FITS_SIGNUPSIGNIN/v2.0/.well-known/openid-configuration\ndocs: https://www.phillips66.com/midstream/customers/\nnote: >-\n  DCP Midstream publishes NO developer API and therefore no API authentication\n  contract. What it does publish is the identity layer in front of its\n  login-gated customer systems, and that layer is machine-readable: two OpenID\n  Connect discovery documents on Phillips 66 Midstream's own Azure AD B2C tenant.\n  Everything below is read from those documents and from the sign-in links on the\n  Midstream customer-tools page — nothing here is derived from an OpenAPI,\n  because none exists. This profile describes HUMAN sign-in to customer portals,\n  not programmatic API access; no client-credentials or machine-to-machine flow\n  is advertised anywhere on the public surface.\nsummary:\n  types: [openIdConnect]\n  api_key_in: []\n\
  \  oauth2_flows: [authorizationCode]\n  pkce: true\n  machine_to_machine: false\n  developer_api_auth: none\nschemes:\n  - name: fits-b2c\n    type: openIdConnect\n    system: FITS (Field Information & Technology Services)\n    application: https://fits.ephillips66.com/\n    openIdConnectUrl: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/B2C_1A_FITS_SIGNUPSIGNIN/v2.0/.well-known/openid-configuration\n    issuer: https://azrmdstadb2cr5.b2clogin.com/e1fdebb4-638c-48e6-b771-2413e270655c/v2.0/\n    provider: Azure AD B2C\n    policy: B2C_1A_FITS_SIGNUPSIGNIN\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/b2c_1a_fits_signupsignin/oauth2/authorize\n        tokenUrl: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/b2c_1a_fits_signupsignin/oauth2/token\n        pkce: S256\n    jwks_uri: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/b2c_1a_fits_signupsignin/discovery/keys\n\
  \    end_session_endpoint: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/b2c_1a_fits_signupsignin/oauth2/logout\n    scopes_supported: [openid]\n    id_token_signing_alg_values_supported: [RS256]\n    subject_types_supported: [pairwise]\n    claims_supported:\n      - email\n      - sub\n      - tid\n      - given_name\n      - family_name\n      - name\n      - businessPhone\n      - companyName\n      - newUser\n      - termsOfUseVersionAccepted\n    sources: [well-known/dcp-midstream-partners-fits-openid-configuration.json]\n  - name: aligne-b2c\n    type: openIdConnect\n    system: Aligne — natural gas scheduling, customer activities & informational postings\n    application: https://alnlogin.ephillips66.com/\n    openIdConnectUrl: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/B2C_1A_ALIGNEAPP_SIGNUPSIGNIN/v2.0/.well-known/openid-configuration\n    issuer: https://azrmdstadb2cr5.b2clogin.com/e1fdebb4-638c-48e6-b771-2413e270655c/v2.0/\n    provider:\
  \ Azure AD B2C\n    policy: B2C_1A_ALIGNEAPP_SIGNUPSIGNIN\n    relying_party: https://azrmdstadb2cr5.onmicrosoft.com/AligneApp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/b2c_1a_aligneapp_signupsignin/oauth2/authorize\n        tokenUrl: https://azrmdstadb2cr5.b2clogin.com/azrmdstadb2cr5.onmicrosoft.com/b2c_1a_aligneapp_signupsignin/oauth2/token\n    scopes_supported: [openid]\n    claims_supported:\n      - SubjectNamingInfo\n      - objectId\n      - businessPhone\n      - companyName\n      - newUser\n      - termsOfUseVersionAccepted\n    sources: [well-known/dcp-midstream-partners-aligne-openid-configuration.json]\nother_gated_systems:\n  - name: TIPS / MyQuorum (plant accounting, CDP monthly allocations, revenue reports)\n    url: https://revenuereporting.ephillips66.com/MYQUORUM_PROD\n    auth: HTTP 401 on every anonymous request; scheme not published\n  - name: Midstream Customer Service\
  \ Portal (ServiceNow)\n    url: https://p66.service-now.com/midstreamcsm\n    auth: ServiceNow-hosted; vendor-operated, not a DCP-authored contract\naccess_request:\n  process: Access is requested from a DCP Gas Logistics scheduler or the support desks\n  contacts:\n    - fits@p66.com\n    - NaturalGasScheduling@p66.com\n  phone: 1-800-909-3487\n  self_service_signup: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dcp-midstream-partners/refs/heads/main/authentication/dcp-midstream-partners-authentication.yml
summary_line: openIdConnect · 2 schemes
tags:
- Energy
- Midstream
- Natural Gas
- Natural Gas Liquids
- Oil and Gas
- Pipelines
---
