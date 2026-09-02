---
api_key_in: []
api_specs:
- filename: shanghai-jiao-tong-university-open-api-openapi.yml
  format: yaml
  label: SJTU Open API
  slug: open-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shanghai-jiao-tong-university/refs/heads/main/openapi/shanghai-jiao-tong-university-open-api-openapi.yml
- filename: shanghai-jiao-tong-university-data-resources-openapi.yml
  format: yaml
  label: SJTU Data Resources API
  slug: data-resources
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/shanghai-jiao-tong-university/refs/heads/main/openapi/shanghai-jiao-tong-university-data-resources-openapi.yml
auth_types:
- oauth2
- openIdConnect
- saml2
- totp
description: ''
kind: authentication
layout: security
method: derived
name: Shanghai Jiao Tong University Authentication
name_suffix: Authentication
oauth_flows: []
overview: Shanghai Jiao Tong University secures its APIs with oauth2, openIdConnect, saml2, and totp across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Shanghai Jiao Tong University
provider_slug: shanghai-jiao-tong-university
scheme_count: 4
schemes:
- description: 'OAuth 2.0 authorization server run by SJTU. Access tokens may be presented either as an access_token query-string or body parameter, or as an Authorization: Bearer header per RFC 6750. Which grants an operation accepts is documented per operation; the portal marks them 授权码 (authorization code, A), 客户端 (client credentials, C) and 密码 (resource-owner password, P).'
  flows:
  - authorizationUrl: https://jaccount.sjtu.edu.cn/oauth2/authorize
    flow: authorizationCode
    pkce: not advertised
    tokenUrl: https://jaccount.sjtu.edu.cn/oauth2/token
  - flow: clientCredentials
    tokenUrl: https://jaccount.sjtu.edu.cn/oauth2/token
  - flow: password
    note: Resource-owner password credentials is still offered and is the documented grant for a handful of notification and mail operations. It is deprecated in OAuth 2.1 and its presence is a real, dateable observation about this platform rather than a criticism of the institution.
    tokenUrl: https://jaccount.sjtu.edu.cn/oauth2/token
  issuer: https://jaccount.sjtu.edu.cn/oauth2/
  name: jAccountOAuth2
  sources:
  - well-known/shanghai-jiao-tong-university-openid-configuration.json
  type: oauth2
- description: 'OpenID Connect on top of the same authorization server. The ID token is a JWT carrying iss, sub (the jAccount name), aud, nonce, exp, iat, name (the user''s real name), code (the default identity''s student/staff number) and type (the default identity type). Three login patterns are documented: authorization-code OIDC, implicit OIDC, and an authorization-code plus Profile API pattern that returns more user detail than the ID token carries.'
  discovery:
    authorization_endpoint: https://jaccount.sjtu.edu.cn/oauth2/authorize
    end_session_endpoint: null
    id_token_signing_alg_values_supported:
    - HS256
    issuer: https://jaccount.sjtu.edu.cn/oauth2/
    jwks_uri: null
    response_types_supported:
    - code
    - code id_token
    - id_token
    - id_token token
    scopes_supported:
    - openid
    - basic
    subject_types_supported:
    - public
    token_endpoint: https://jaccount.sjtu.edu.cn/oauth2/token
    userinfo_endpoint: null
  gaps:
  - id_token_signing_alg_values_supported is HS256 only. The ID token is symmetrically signed with the client_secret, so there is no JWKS to publish and no asymmetric verification path — a public client (SPA, mobile app) cannot verify an ID token without embedding the secret.
  - No jwks_uri, userinfo_endpoint, registration_endpoint, introspection_endpoint, revocation_endpoint or end_session_endpoint is advertised, and no code_challenge_methods_supported (PKCE) is declared. The portal documents application logout separately in prose.
  - scopes_supported advertises only openid and basic, while the portal's authorization-scope table documents 39 scopes. The discovery document under-reports the platform.
  name: jAccountOIDC
  openIdConnectUrl: https://jaccount.sjtu.edu.cn/oauth2/.well-known/openid-configuration
  sources:
  - well-known/shanghai-jiao-tong-university-openid-configuration.json
  type: openIdConnect
- description: Shibboleth identity provider publishing SAML 2.0 metadata. This is the surface that federates SJTU into CARSI (CERNET Authentication and Resource Sharing Infrastructure), which has been a full member of eduGAIN since 2019 — so an SJTU account authenticates against licensed resources worldwide through this entity.
  display_name: SJTU Identity Provider
  endpoints:
    attribute_query:
    - binding: urn:oasis:names:tc:SAML:1.0:bindings:SOAP-binding
      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML1/SOAP/AttributeQuery
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP
      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/SOAP/AttributeQuery
    single_logout:
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/Redirect/SLO
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/POST/SLO
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign
      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/POST-SimpleSign/SLO
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP
      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/SOAP/SLO
    single_sign_on:
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/POST/SSO
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign
      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/POST-SimpleSign/SSO
    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/Redirect/SSO
    - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest
      location: https://jaccount.sjtu.edu.cn/idp/profile/Shibboleth/SSO
  entity_id: https://jaccount.sjtu.edu.cn/idp/shibboleth
  metadata_url: https://jaccount.sjtu.edu.cn/idp/shibboleth
  name: jAccountShibbolethIdP
  observations:
  - The signing certificate in the metadata was issued 2016-10-01 and does not expire until 2036-10-01 — a twenty-year self-signed IdP certificate, which is conventional for Shibboleth metadata but worth recording.
  - Apache-Coyote/1.1 is returned in the Server header, so the IdP is running on an old Tomcat connector generation.
  protocols:
  - urn:oasis:names:tc:SAML:2.0:protocol
  - urn:oasis:names:tc:SAML:1.1:protocol
  - urn:mace:shibboleth:1.0
  scope: sjtu.edu.cn
  sources:
  - well-known/shanghai-jiao-tong-university-saml-idp-metadata.xml
  type: saml2
- description: Dynamic one-time password (动态口令), documented at /auth/totp.html as a second factor alongside jAccount password login.
  name: jAccountTOTP
  sources:
  - https://developer.sjtu.edu.cn/auth/totp.html
  type: totp
slug: shanghai-jiao-tong-university-authentication
source_filename: shanghai-jiao-tong-university-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: derived\nx-evidence-method: probed\nx-authorship: >-\n  Written by API Evangelist from live probes of SJTU's own hosts plus SJTU's own published\n  documentation. Not authored or published by Shanghai Jiao Tong University.\nsource: https://jaccount.sjtu.edu.cn/oauth2/.well-known/openid-configuration\ndocs:\n- https://developer.sjtu.edu.cn/auth/oidc.html\n- https://developer.sjtu.edu.cn/auth/oauth.html\n- https://developer.sjtu.edu.cn/auth/jaccount.html\n- https://developer.sjtu.edu.cn/auth/totp.html\nx-operator: institution\nnote: >-\n  jAccount is Shanghai Jiao Tong University's own identity provider, operated by the SJTU Network\n  and Information Center on the university's own domain. It is not a vendor tenancy: the OAuth 2.0\n  authorization server, the OpenID Connect provider and the Shibboleth SAML identity provider all\n  run under jaccount.sjtu.edu.cn and are documented on the university's own developer portal. Every\n  programmable\
  \ surface SJTU operates — the Open API at api.sjtu.edu.cn, the Data Resources API at\n  graphql.sjtu.edu.cn, and the 交我办 process platform — authenticates through it.\nsummary:\n  types: [oauth2, openIdConnect, saml2, totp]\n  discovery_published: true\n  standards: [oauth2, oidc, saml2, shibboleth, rfc6749, rfc6750, jwt]\nschemes:\n- name: jAccountOAuth2\n  type: oauth2\n  description: >-\n    OAuth 2.0 authorization server run by SJTU. Access tokens may be presented either as an\n    access_token query-string or body parameter, or as an Authorization: Bearer header per RFC 6750.\n    Which grants an operation accepts is documented per operation; the portal marks them 授权码\n    (authorization code, A), 客户端 (client credentials, C) and 密码 (resource-owner password, P).\n  issuer: https://jaccount.sjtu.edu.cn/oauth2/\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://jaccount.sjtu.edu.cn/oauth2/authorize\n    tokenUrl: https://jaccount.sjtu.edu.cn/oauth2/token\n    pkce:\
  \ not advertised\n  - flow: clientCredentials\n    tokenUrl: https://jaccount.sjtu.edu.cn/oauth2/token\n  - flow: password\n    tokenUrl: https://jaccount.sjtu.edu.cn/oauth2/token\n    note: >-\n      Resource-owner password credentials is still offered and is the documented grant for a\n      handful of notification and mail operations. It is deprecated in OAuth 2.1 and its presence\n      is a real, dateable observation about this platform rather than a criticism of the institution.\n  sources: [well-known/shanghai-jiao-tong-university-openid-configuration.json]\n- name: jAccountOIDC\n  type: openIdConnect\n  description: >-\n    OpenID Connect on top of the same authorization server. The ID token is a JWT carrying iss,\n    sub (the jAccount name), aud, nonce, exp, iat, name (the user's real name), code (the default\n    identity's student/staff number) and type (the default identity type). Three login patterns are\n    documented: authorization-code OIDC, implicit OIDC, and an authorization-code\
  \ plus Profile API\n    pattern that returns more user detail than the ID token carries.\n  openIdConnectUrl: https://jaccount.sjtu.edu.cn/oauth2/.well-known/openid-configuration\n  discovery:\n    issuer: https://jaccount.sjtu.edu.cn/oauth2/\n    authorization_endpoint: https://jaccount.sjtu.edu.cn/oauth2/authorize\n    token_endpoint: https://jaccount.sjtu.edu.cn/oauth2/token\n    response_types_supported: [code, code id_token, id_token, id_token token]\n    subject_types_supported: [public]\n    id_token_signing_alg_values_supported: [HS256]\n    scopes_supported: [openid, basic]\n    jwks_uri: null\n    userinfo_endpoint: null\n    end_session_endpoint: null\n  gaps:\n  - >-\n    id_token_signing_alg_values_supported is HS256 only. The ID token is symmetrically signed with\n    the client_secret, so there is no JWKS to publish and no asymmetric verification path — a public\n    client (SPA, mobile app) cannot verify an ID token without embedding the secret.\n  - >-\n    No jwks_uri,\
  \ userinfo_endpoint, registration_endpoint, introspection_endpoint,\n    revocation_endpoint or end_session_endpoint is advertised, and no code_challenge_methods_supported\n    (PKCE) is declared. The portal documents application logout separately in prose.\n  - >-\n    scopes_supported advertises only openid and basic, while the portal's authorization-scope table\n    documents 39 scopes. The discovery document under-reports the platform.\n  sources: [well-known/shanghai-jiao-tong-university-openid-configuration.json]\n- name: jAccountShibbolethIdP\n  type: saml2\n  description: >-\n    Shibboleth identity provider publishing SAML 2.0 metadata. This is the surface that federates\n    SJTU into CARSI (CERNET Authentication and Resource Sharing Infrastructure), which has been a\n    full member of eduGAIN since 2019 — so an SJTU account authenticates against licensed resources\n    worldwide through this entity.\n  entity_id: https://jaccount.sjtu.edu.cn/idp/shibboleth\n  metadata_url:\
  \ https://jaccount.sjtu.edu.cn/idp/shibboleth\n  scope: sjtu.edu.cn\n  display_name: SJTU Identity Provider\n  protocols:\n  - urn:oasis:names:tc:SAML:2.0:protocol\n  - urn:oasis:names:tc:SAML:1.1:protocol\n  - urn:mace:shibboleth:1.0\n  endpoints:\n    single_sign_on:\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/POST/SSO\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/POST-SimpleSign/SSO\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/Redirect/SSO\n    - binding: urn:mace:shibboleth:1.0:profiles:AuthnRequest\n      location: https://jaccount.sjtu.edu.cn/idp/profile/Shibboleth/SSO\n    single_logout:\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/Redirect/SLO\n\
  \    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/POST/SLO\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/POST-SimpleSign/SLO\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/SOAP/SLO\n    attribute_query:\n    - binding: urn:oasis:names:tc:SAML:1.0:bindings:SOAP-binding\n      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML1/SOAP/AttributeQuery\n    - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n      location: https://jaccount.sjtu.edu.cn/idp/profile/SAML2/SOAP/AttributeQuery\n  observations:\n  - >-\n    The signing certificate in the metadata was issued 2016-10-01 and does not expire until\n    2036-10-01 — a twenty-year self-signed IdP certificate, which is conventional for Shibboleth\n    metadata but worth recording.\n  - >-\n\
  \    Apache-Coyote/1.1 is returned in the Server header, so the IdP is running on an old Tomcat\n    connector generation.\n  sources: [well-known/shanghai-jiao-tong-university-saml-idp-metadata.xml]\n- name: jAccountTOTP\n  type: totp\n  description: >-\n    Dynamic one-time password (动态口令), documented at /auth/totp.html as a second factor alongside\n    jAccount password login.\n  sources: [https://developer.sjtu.edu.cn/auth/totp.html]\nonboarding:\n  self_service: false\n  detail: >-\n    There is no self-service developer signup. An application is registered by signing in to\n    my.sjtu.edu.cn or the 交我办 app and following Service Hall -> Information Services -> jAccount\n    interface application (服务大厅 -> 信息服务 -> jAccount接口申请). Approval issues an appId (of the\n    form japortal000000) and a 48-character appSecret. Adding a scope after the fact requires an\n    email to the platform contact naming the appId and the new scope codes. Data Resources access\n    additionally requires\
  \ the separate 数据资源申请流程.\n  eligibility: >-\n    A jAccount is required to submit the application, so the developer audience is university\n    members and their partners, not the general public.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/shanghai-jiao-tong-university/refs/heads/main/authentication/shanghai-jiao-tong-university-authentication.yml
summary_line: oauth2/openIdConnect/saml2/totp · 4 schemes
tags:
- University
- Higher Education
- Education
- Research
- China
- C9 League
- Identity Federation
- Course Catalog
- Research Computing
- Campus Life
- Authentication
- OpenID Connect
- SAML
- Shibboleth
- Payments
---
