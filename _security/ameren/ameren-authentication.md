---
api_key_in: []
auth_types: []
description: 'Ameren publishes no OpenAPI, so this profile is not derived from a spec. It is read from two real sources: (1) the live, anonymous OpenID Connect discovery document served by Ameren''s ForgeRock AM enterprise identity service (eiam = Enterprise Identity and Access Management) at login.eiam.ece.ameren.com, and (2) Ameren Illinois'' own Share My Usage program page, which states the program uses the Green Button Connect My Data APIs with OAuth customer authorization and that Aclara is the authorized data custodian.'
kind: authentication
layout: security
method: probed
name: Ameren Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ameren declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Ameren
provider_slug: ameren
scheme_count: 2
schemes:
- caveat: The advertised endpoint host global.login.eiam.ameren.com does not resolve publicly. The discovery document is anonymously readable; the endpoints it names are not publicly reachable. Treat the endpoint list as declared configuration, not as a callable public surface.
  claims:
  - name
  - given_name
  - family_name
  - email
  - phone_number
  - address
  - profile
  - locale
  - zoneinfo
  endpoints:
    authorization: https://global.login.eiam.ameren.com/am/oauth2/authorize
    check_session_iframe: https://global.login.eiam.ameren.com/am/oauth2/connect/checkSession
    end_session: https://global.login.eiam.ameren.com/am/oauth2/connect/endSession
    introspection: https://global.login.eiam.ameren.com/am/oauth2/introspect
    jwks: https://global.login.eiam.ameren.com/am/oauth2/connect/jwk_uri
    pushed_authorization_request: https://global.login.eiam.ameren.com/am/oauth2/par
    registration: https://global.login.eiam.ameren.com/am/oauth2/register
    revocation: https://global.login.eiam.ameren.com/am/oauth2/token/revoke
    token: https://global.login.eiam.ameren.com/am/oauth2/access_token
    userinfo: https://global.login.eiam.ameren.com/am/oauth2/userinfo
  grant_types:
  - authorization_code
  - implicit
  - refresh_token
  - password
  - client_credentials
  - urn:ietf:params:oauth:grant-type:device_code
  - urn:ietf:params:oauth:grant-type:saml2-bearer
  - urn:ietf:params:oauth:grant-type:uma-ticket
  id: ameren_eiam_oidc
  id_token_signing_algs:
  - RS256
  - RS384
  - RS512
  - PS256
  - PS384
  - PS512
  - ES256
  - ES384
  - ES512
  - HS256
  - HS384
  - HS512
  issuer: https://global.login.eiam.ameren.com/am/oauth2
  mutual_tls:
    certificate_bound_access_tokens: false
    client_auth: true
  name: Ameren Enterprise IAM (ForgeRock AM)
  openIdConnectUrl: https://login.eiam.ece.ameren.com/am/oauth2/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    - plain
    supported: true
  pushed_authorization_requests:
    required: false
    supported: true
  response_types:
  - code
  - token
  - id_token
  - code id_token
  - code token
  - token id_token
  - code token id_token
  - device_code
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - private_key_jwt
  - tls_client_auth
  - self_signed_tls_client_auth
  - none
  type: openIdConnect
- description: 'Ameren Illinois'' Share My Usage program follows the NAESB/ESPI Green Button Connect My Data profile: the customer signs in to their Ameren Illinois online account and authorizes a registered third party, which then retrieves up to 24 months of historical and 24 months of forward electric usage data as ESPI XML. Ameren Illinois'' page states the technical requirements are "consistent with those defined in the standard Green Button Connect Application Programming Interfaces."'
  endpoints_note: NEITHER Ameren nor Aclara publishes the OAuth authorize/token URLs or the ESPI resource base for this program on any public page. They are handed to a third party by Aclara during the 2-4 week registration. The canonical Green Button DataCustodian resource path was probed on gp.ameren.com and returned the site's HTML bot-challenge page, not an ESPI Atom feed.
  endpoints_published: false
  id: green_button_oauth
  method: searched
  name: Green Button Connect My Data (Share My Usage) customer authorization
  onboarding:
    contact: IllinoisBusinessApplications@ameren.com
    custodian: Aclara
    duration: 2 to 4 weeks
    registration_guide_pdf: https://www.ameren.com/-/media/files/resources-and-support/account-and-data/share-usage/third-party-share-my-usage-registration-guide-2019.ashx
    registration_url: https://gp.ameren.com/third-party-registration/instructions
    territory: Illinois only — not available to Missouri customers
  source: https://www.ameren.com/partners/account-and-data/share-my-usage
  type: oauth2
slug: ameren-authentication
source_filename: ameren-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: probed\nsource: https://login.eiam.ece.ameren.com/am/oauth2/.well-known/openid-configuration\ndocs: https://www.ameren.com/partners/account-and-data/share-my-usage\nprovider: Ameren\nproviderId: ameren\ndescription: >-\n  Ameren publishes no OpenAPI, so this profile is not derived from a spec. It is read from\n  two real sources: (1) the live, anonymous OpenID Connect discovery document served by\n  Ameren's ForgeRock AM enterprise identity service (eiam = Enterprise Identity and Access\n  Management) at login.eiam.ece.ameren.com, and (2) Ameren Illinois' own Share My Usage\n  program page, which states the program uses the Green Button Connect My Data APIs with\n  OAuth customer authorization and that Aclara is the authorized data custodian.\nownership: >-\n  The discovery document's issuer and every advertised endpoint are on\n  global.login.eiam.ameren.com — an ameren.com host — so this identity surface belongs to\n  Ameren and not to a vendor\
  \ tenant.\nschemes:\n  - id: ameren_eiam_oidc\n    type: openIdConnect\n    name: Ameren Enterprise IAM (ForgeRock AM)\n    openIdConnectUrl: https://login.eiam.ece.ameren.com/am/oauth2/.well-known/openid-configuration\n    issuer: https://global.login.eiam.ameren.com/am/oauth2\n    endpoints:\n      authorization: https://global.login.eiam.ameren.com/am/oauth2/authorize\n      token: https://global.login.eiam.ameren.com/am/oauth2/access_token\n      userinfo: https://global.login.eiam.ameren.com/am/oauth2/userinfo\n      jwks: https://global.login.eiam.ameren.com/am/oauth2/connect/jwk_uri\n      introspection: https://global.login.eiam.ameren.com/am/oauth2/introspect\n      revocation: https://global.login.eiam.ameren.com/am/oauth2/token/revoke\n      registration: https://global.login.eiam.ameren.com/am/oauth2/register\n      pushed_authorization_request: https://global.login.eiam.ameren.com/am/oauth2/par\n      end_session: https://global.login.eiam.ameren.com/am/oauth2/connect/endSession\n\
  \      check_session_iframe: https://global.login.eiam.ameren.com/am/oauth2/connect/checkSession\n    grant_types:\n      - authorization_code\n      - implicit\n      - refresh_token\n      - password\n      - client_credentials\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:saml2-bearer\n      - urn:ietf:params:oauth:grant-type:uma-ticket\n    response_types:\n      - code\n      - token\n      - id_token\n      - code id_token\n      - code token\n      - token id_token\n      - code token id_token\n      - device_code\n    token_endpoint_auth_methods:\n      - client_secret_basic\n      - client_secret_post\n      - private_key_jwt\n      - tls_client_auth\n      - self_signed_tls_client_auth\n      - none\n    pkce:\n      supported: true\n      code_challenge_methods: [S256, plain]\n    mutual_tls:\n      client_auth: true\n      certificate_bound_access_tokens: false\n    pushed_authorization_requests:\n      supported: true\n   \
  \   required: false\n    id_token_signing_algs: [RS256, RS384, RS512, PS256, PS384, PS512, ES256, ES384, ES512, HS256, HS384, HS512]\n    subject_types: [public]\n    claims: [name, given_name, family_name, email, phone_number, address, profile, locale, zoneinfo]\n    caveat: >-\n      The advertised endpoint host global.login.eiam.ameren.com does not resolve publicly.\n      The discovery document is anonymously readable; the endpoints it names are not\n      publicly reachable. Treat the endpoint list as declared configuration, not as a\n      callable public surface.\n  - id: green_button_oauth\n    type: oauth2\n    name: Green Button Connect My Data (Share My Usage) customer authorization\n    method: searched\n    source: https://www.ameren.com/partners/account-and-data/share-my-usage\n    description: >-\n      Ameren Illinois' Share My Usage program follows the NAESB/ESPI Green Button Connect\n      My Data profile: the customer signs in to their Ameren Illinois online account\
  \ and\n      authorizes a registered third party, which then retrieves up to 24 months of\n      historical and 24 months of forward electric usage data as ESPI XML. Ameren Illinois'\n      page states the technical requirements are \"consistent with those defined in the\n      standard Green Button Connect Application Programming Interfaces.\"\n    endpoints_published: false\n    endpoints_note: >-\n      NEITHER Ameren nor Aclara publishes the OAuth authorize/token URLs or the ESPI\n      resource base for this program on any public page. They are handed to a third party\n      by Aclara during the 2-4 week registration. The canonical Green Button DataCustodian\n      resource path was probed on gp.ameren.com and returned the site's HTML bot-challenge\n      page, not an ESPI Atom feed.\n    onboarding:\n      registration_url: https://gp.ameren.com/third-party-registration/instructions\n      registration_guide_pdf: https://www.ameren.com/-/media/files/resources-and-support/account-and-data/share-usage/third-party-share-my-usage-registration-guide-2019.ashx\n\
  \      contact: IllinoisBusinessApplications@ameren.com\n      duration: 2 to 4 weeks\n      custodian: Aclara\n      territory: Illinois only — not available to Missouri customers\napi_key_support: false\nmutual_tls_only: false\nevidence:\n  - url: https://login.eiam.ece.ameren.com/am/oauth2/.well-known/openid-configuration\n    status: 200\n    kind: OIDC discovery document (anonymous)\n  - url: https://login.eiam.ece.ameren.com/am/oauth2/connect/jwk_uri\n    status: 200\n    kind: JWKS\n  - url: https://login.eiam.ece.ameren.com/.well-known/openid-configuration\n    status: 404\n    kind: RFC 8414 root path (not served)\n  - url: https://www.ameren.com/partners/account-and-data/share-my-usage\n    status: 200\n    kind: program documentation\n  - url: https://gp.ameren.com/DataCustodian/espi/1_1/resource/ApplicationInformation\n    status: 200\n    kind: MISS — HTML bot-challenge page, not ESPI\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ameren/refs/heads/main/authentication/ameren-authentication.yml
summary_line: 2 schemes
tags:
- Utility
- Energy
- Electric
- Natural Gas
- Smart Grid
- Green Button
- Renewable Energy
- Fortune 500
---
