---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Ofgem Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Ofgem secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Ofgem
provider_slug: ofgem
scheme_count: 2
schemes:
- anonymous_read_note: Authentication is not enforced on all of the backing GraphQL endpoint - several read operations return real register content anonymously (see graphql/ofgem-epr-graphql.yml). Sign-in gates the licence-modification proposal workflow and user-scoped data.
  application: https://epr.ofgem.gov.uk/
  authorizationUrl: https://epre-api.ofgem.gov.uk/authenticate/
  clientId: 55o2cl3csa5ab7rctka6de5rvp
  discovery: None served. https://ofgem-live-portal.auth.eu-west-2.amazoncognito.com/.well-known/openid-configuration returned 404 and the user-pool issuer is not published, so no OIDC metadata is obtainable for this application.
  flow: authorizationCode
  logoutUrl: https://ofgem-live-portal.auth.eu-west-2.amazoncognito.com/logout
  name: EPR (Electronic Public Register) - AWS Cognito
  pkce: true
  redirectUri: https://epr.ofgem.gov.uk
  scopes:
  - openid
  - profile
  - email
  source: https://epr.ofgem.gov.uk/ofgem-live-v4.20.31-28588873106-3-1/index.js
  tokenUrl: https://epre-api.ofgem.gov.uk/tokens/
  token_storage: browser storage key ROCP_token (bearer, client-side)
  type: oauth2
- anonymous_read_note: None. Every RER path probed, including the pages Ofgem calls "public reports", 302-redirects to the B2C sign-in. The register is entirely account-gated.
  application: https://rer.ofgem.gov.uk/
  authorizationUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/oauth2/v2.0/authorize
  clientId: 05624aa9-bc87-4076-88c3-fd451bb29006
  code_challenge_method: S256
  discovery_file: well-known/ofgem-rer-openid-configuration.json
  endSessionUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/oauth2/v2.0/logout
  flow: authorizationCode
  id_token_signing_alg:
  - RS256
  issuer: https://pk8sprdofgemcloudb2c.b2clogin.com/66336e89-d63b-4197-98af-792db50aa4aa/v2.0/
  jwksUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/discovery/v2.0/keys
  name: RER (Renewable Electricity Register) - Azure AD B2C
  openIdConnectUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/v2.0/.well-known/openid-configuration
  pkce: true
  scopes:
  - openid
  - profile
  - offline_access
  - https://pk8sprdofgemcloudb2c.onmicrosoft.com/rercoreservices/user_impersonation
  source: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/v2.0/.well-known/openid-configuration
  subject_types:
  - pairwise
  tokenUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/oauth2/v2.0/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: openIdConnect
  user_flow: b2c_1a_rer_signin (custom policy)
slug: ofgem-authentication
source_filename: ofgem-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  Live anonymous probes and the two register applications' own published JavaScript\n  configuration, 2026-07-27. No OpenAPI exists for this provider, so nothing here is\n  derived from a specification.\ndocs: null\nsummary:\n  public_api_auth: none\n  public_api_auth_detail: >-\n    Ofgem publishes no API, so there is no public authentication model, no key\n    request route, no client registration and no token endpoint a developer may use.\n    Everything below describes the identity layer in front of Ofgem's two internal\n    register applications, discovered by probing - not a developer-facing contract.\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  pkce: true\n  discovery_documents: 1\nschemes:\n- name: EPR (Electronic Public Register) - AWS Cognito\n  application: https://epr.ofgem.gov.uk/\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  authorizationUrl: https://epre-api.ofgem.gov.uk/authenticate/\n\
  \  tokenUrl: https://epre-api.ofgem.gov.uk/tokens/\n  logoutUrl: https://ofgem-live-portal.auth.eu-west-2.amazoncognito.com/logout\n  redirectUri: https://epr.ofgem.gov.uk\n  clientId: 55o2cl3csa5ab7rctka6de5rvp\n  scopes: [openid, profile, email]\n  token_storage: browser storage key ROCP_token (bearer, client-side)\n  discovery: >-\n    None served. https://ofgem-live-portal.auth.eu-west-2.amazoncognito.com/.well-known/openid-configuration\n    returned 404 and the user-pool issuer is not published, so no OIDC metadata is\n    obtainable for this application.\n  source: https://epr.ofgem.gov.uk/ofgem-live-v4.20.31-28588873106-3-1/index.js\n  anonymous_read_note: >-\n    Authentication is not enforced on all of the backing GraphQL endpoint - several\n    read operations return real register content anonymously (see\n    graphql/ofgem-epr-graphql.yml). Sign-in gates the licence-modification proposal\n    workflow and user-scoped data.\n- name: RER (Renewable Electricity Register) - Azure\
  \ AD B2C\n  application: https://rer.ofgem.gov.uk/\n  type: openIdConnect\n  flow: authorizationCode\n  pkce: true\n  code_challenge_method: S256\n  openIdConnectUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/v2.0/.well-known/openid-configuration\n  discovery_file: well-known/ofgem-rer-openid-configuration.json\n  issuer: https://pk8sprdofgemcloudb2c.b2clogin.com/66336e89-d63b-4197-98af-792db50aa4aa/v2.0/\n  authorizationUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/oauth2/v2.0/authorize\n  tokenUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/oauth2/v2.0/token\n  endSessionUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/oauth2/v2.0/logout\n  jwksUrl: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/discovery/v2.0/keys\n  user_flow:\
  \ b2c_1a_rer_signin (custom policy)\n  clientId: 05624aa9-bc87-4076-88c3-fd451bb29006\n  scopes: [openid, profile, offline_access, 'https://pk8sprdofgemcloudb2c.onmicrosoft.com/rercoreservices/user_impersonation']\n  id_token_signing_alg: [RS256]\n  token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n  subject_types: [pairwise]\n  anonymous_read_note: >-\n    None. Every RER path probed, including the pages Ofgem calls \"public reports\",\n    302-redirects to the B2C sign-in. The register is entirely account-gated.\n  source: https://pk8sprdofgemcloudb2c.b2clogin.com/pk8sprdofgemcloudb2c.onmicrosoft.com/b2c_1a_rer_signin/v2.0/.well-known/openid-configuration\nopen_data_access:\n  gate: none\n  detail: >-\n    The Ofgem Data Portal, the price-cap workbooks, the FIT and REGO reports and the\n    data release calendar are all anonymous file downloads (CSV, XLSX, PNG). No\n    account, no key, no licence click-through and no rate limit applies - and no\n    interface either.\n\
  inbound_only_surface:\n  name: Ofgem Data Exchange Service (Beta)\n  direction: inbound (industry submits returns to Ofgem)\n  auth: not published\n  access: invitation only; contact ofgemdataservices@ofgem.gov.uk\n  note: >-\n    Ofgem's guidance page states the Beta supports automating file submission\n    \"including via API\" but publishes no hostname, contract or self-service route;\n    dataexchange.ofgem.gov.uk does not resolve.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ofgem/refs/heads/main/authentication/ofgem-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Energy
- United Kingdom
- Utilities
- Electricity
- Gas
- Energy Markets
- Regulator
- Smart Metering
- Open Data
- Energy Regulation
- Renewables
- Great Britain
---
