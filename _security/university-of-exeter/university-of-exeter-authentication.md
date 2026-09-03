---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- saml2
- token
description: ''
kind: authentication
layout: security
method: probed
name: University Of Exeter Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Exeter secures its APIs with oauth2, openIdConnect, saml2, and token across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Exeter
provider_slug: university-of-exeter
scheme_count: 5
schemes:
- applies_to: https://api.exeter.ac.uk
  authorizationUrl: https://exeter-auth-prod.auth.eu-west-2.amazoncognito.com/oauth2/authorize
  description: The MyExeter platform API is protected by an Exeter-owned AWS Cognito user pool in eu-west-2. Unauthenticated requests to existing routes return 401 {"message":"Unauthorized"}; unrouted paths return the API Gateway default 403 {"message":"Missing Authentication Token"}, which is how the route inventory was confirmed. Some routes additionally require a `tenant` request header - /application-settings returns 400 BAD_REQUEST "tenant is required" without it.
  flows:
  - authorizationCode
  name: cognitoOAuth2
  sources:
  - https://m.exeter.ac.uk/main.dart.js
  - https://api.exeter.ac.uk/user/profile
  tokenUrl: https://exeter-auth-prod.auth.eu-west-2.amazoncognito.com/oauth2/token
  type: oauth2
- applies_to: Exeter staff and student single sign-on
  description: Exeter's Microsoft Entra ID tenant publishes OIDC discovery metadata (200, application/json) advertising token_endpoint, jwks_uri and token_endpoint_auth_methods_supported of client_secret_post, private_key_jwt, client_secret_basic and self_signed_tls_client_auth. Application registration in this tenant is closed to the public.
  name: entraIdOidc
  openIdConnectUrl: https://login.microsoftonline.com/912a5d77-fb98-4eee-af32-1334d8f04a53/v2.0/.well-known/openid-configuration
  sources:
  - https://login.microsoftonline.com/912a5d77-fb98-4eee-af32-1334d8f04a53/v2.0/.well-known/openid-configuration
  type: openIdConnect
- applies_to: Library electronic resources and federated service providers
  description: Exeter's own Shibboleth 2.0 identity provider. SSO is offered over HTTP-Redirect, HTTP-POST, HTTP-POST-SimpleSign and SOAP/ECP; SLO and ArtifactResolution are advertised. Access is granted to service providers registered in the UK Access Management Federation or reachable through eduGAIN, not to individual developers.
  entityId: https://elibrary.exeter.ac.uk/idp/shibboleth
  federations:
  - http://mdq.ukfederation.org.uk/entities/https%3A%2F%2Felibrary.exeter.ac.uk%2Fidp%2Fshibboleth
  - https://mdq.incommon.org/entities/https%3A%2F%2Felibrary.exeter.ac.uk%2Fidp%2Fshibboleth
  metadataUrl: https://elibrary.exeter.ac.uk/idp/shibboleth
  name: shibbolethSaml
  sources:
  - https://elibrary.exeter.ac.uk/idp/shibboleth
  type: saml2
- applies_to: https://ele.exeter.ac.uk/webservice/rest/server.php
  description: Moodle web services are enabled on ELE and gated by a per-user web-service token. An unauthenticated request returns a well-formed Moodle exception (ERRORCODE invalidtoken, "Invalid token - token not found") rather than a 404, which is how the surface was confirmed. Tokens are issued to affiliated users through Moodle, not through any public registration.
  in: query
  name: moodleWebServiceToken
  parameterName: wstoken
  sources:
  - https://ele.exeter.ac.uk/webservice/rest/server.php
  type: token
- applies_to: LTI 1.3 tools launching into ELE
  authorizationUrl: https://ele.exeter.ac.uk/mod/lti/auth.php
  description: ELE acts as an LTI 1.3 Advantage tool platform. It publishes an RSA JWKS at /mod/lti/certs.php, an OIDC authorization endpoint at /mod/lti/auth.php, and the Advantage services endpoint at /mod/lti/services.php. Tool deployments are registered by Exeter, not self-service.
  jwksUrl: https://ele.exeter.ac.uk/mod/lti/certs.php
  name: ltiAdvantage
  sources:
  - https://ele.exeter.ac.uk/mod/lti/certs.php
  - https://ele.exeter.ac.uk/mod/lti/services.php
  type: openIdConnect
slug: university-of-exeter-authentication
source_filename: university-of-exeter-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes of api.exeter.ac.uk, ele.exeter.ac.uk, elibrary.exeter.ac.uk and the Exeter\n  Entra ID tenant on 2026-09-01, plus the public MyExeter application bundle at\n  https://m.exeter.ac.uk/main.dart.js. Exeter publishes no OpenAPI, so no scheme here is\n  derived from a contract.\nnote: >-\n  Every authenticated surface Exeter operates is credentialed against institutional identity.\n  There is no self-service registration, no API key issuance and no public client\n  registration on any host - an unaffiliated developer cannot obtain a credential for any\n  of these schemes.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - saml2\n  - token\n  self_service: false\n  public_registration: false\nschemes:\n- name: cognitoOAuth2\n  type: oauth2\n  flows:\n  - authorizationCode\n  authorizationUrl: https://exeter-auth-prod.auth.eu-west-2.amazoncognito.com/oauth2/authorize\n  tokenUrl: https://exeter-auth-prod.auth.eu-west-2.amazoncognito.com/oauth2/token\n\
  \  applies_to: https://api.exeter.ac.uk\n  description: >-\n    The MyExeter platform API is protected by an Exeter-owned AWS Cognito user pool in\n    eu-west-2. Unauthenticated requests to existing routes return 401 {\"message\":\"Unauthorized\"};\n    unrouted paths return the API Gateway default 403 {\"message\":\"Missing Authentication Token\"},\n    which is how the route inventory was confirmed. Some routes additionally require a\n    `tenant` request header - /application-settings returns 400 BAD_REQUEST \"tenant is required\"\n    without it.\n  sources:\n  - https://m.exeter.ac.uk/main.dart.js\n  - https://api.exeter.ac.uk/user/profile\n- name: entraIdOidc\n  type: openIdConnect\n  openIdConnectUrl: https://login.microsoftonline.com/912a5d77-fb98-4eee-af32-1334d8f04a53/v2.0/.well-known/openid-configuration\n  applies_to: Exeter staff and student single sign-on\n  description: >-\n    Exeter's Microsoft Entra ID tenant publishes OIDC discovery metadata (200,\n    application/json)\
  \ advertising token_endpoint, jwks_uri and\n    token_endpoint_auth_methods_supported of client_secret_post, private_key_jwt,\n    client_secret_basic and self_signed_tls_client_auth. Application registration in this\n    tenant is closed to the public.\n  sources:\n  - https://login.microsoftonline.com/912a5d77-fb98-4eee-af32-1334d8f04a53/v2.0/.well-known/openid-configuration\n- name: shibbolethSaml\n  type: saml2\n  entityId: https://elibrary.exeter.ac.uk/idp/shibboleth\n  metadataUrl: https://elibrary.exeter.ac.uk/idp/shibboleth\n  applies_to: Library electronic resources and federated service providers\n  description: >-\n    Exeter's own Shibboleth 2.0 identity provider. SSO is offered over HTTP-Redirect,\n    HTTP-POST, HTTP-POST-SimpleSign and SOAP/ECP; SLO and ArtifactResolution are advertised.\n    Access is granted to service providers registered in the UK Access Management Federation\n    or reachable through eduGAIN, not to individual developers.\n  federations:\n  - http://mdq.ukfederation.org.uk/entities/https%3A%2F%2Felibrary.exeter.ac.uk%2Fidp%2Fshibboleth\n\
  \  - https://mdq.incommon.org/entities/https%3A%2F%2Felibrary.exeter.ac.uk%2Fidp%2Fshibboleth\n  sources:\n  - https://elibrary.exeter.ac.uk/idp/shibboleth\n- name: moodleWebServiceToken\n  type: token\n  in: query\n  parameterName: wstoken\n  applies_to: https://ele.exeter.ac.uk/webservice/rest/server.php\n  description: >-\n    Moodle web services are enabled on ELE and gated by a per-user web-service token. An\n    unauthenticated request returns a well-formed Moodle exception\n    (ERRORCODE invalidtoken, \"Invalid token - token not found\") rather than a 404, which is\n    how the surface was confirmed. Tokens are issued to affiliated users through Moodle, not\n    through any public registration.\n  sources:\n  - https://ele.exeter.ac.uk/webservice/rest/server.php\n- name: ltiAdvantage\n  type: openIdConnect\n  jwksUrl: https://ele.exeter.ac.uk/mod/lti/certs.php\n  authorizationUrl: https://ele.exeter.ac.uk/mod/lti/auth.php\n  applies_to: LTI 1.3 tools launching into ELE\n  description:\
  \ >-\n    ELE acts as an LTI 1.3 Advantage tool platform. It publishes an RSA JWKS at\n    /mod/lti/certs.php, an OIDC authorization endpoint at /mod/lti/auth.php, and the\n    Advantage services endpoint at /mod/lti/services.php. Tool deployments are registered by\n    Exeter, not self-service.\n  sources:\n  - https://ele.exeter.ac.uk/mod/lti/certs.php\n  - https://ele.exeter.ac.uk/mod/lti/services.php\nunauthenticated:\n- url: https://news.exeter.ac.uk/wp-json/\n  description: >-\n    The only Exeter-hosted API that serves data without a credential. The WordPress REST API\n    reports an empty `authentication` object and serves /wp/v2/posts openly (X-WP-Total 2,596).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-exeter/refs/heads/main/authentication/university-of-exeter-authentication.yml
summary_line: oauth2/openIdConnect/saml2/token · 5 schemes
tags:
- University
- Higher Education
- Education
- Research
- United Kingdom
- Russell Group
- Identity Federation
- Research Repository
- Learning Management
- Campus Life
---
