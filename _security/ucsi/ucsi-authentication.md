---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- saml2
description: 'What can actually be established about how a client authenticates against anything UCSI University operates. UCSI publishes no public API and no developer documentation, so this artifact describes the one authentication surface that is publicly readable: the OpenID Connect / SAML 2.0 metadata of the institution''s own Microsoft Entra ID tenant. It is a record of a probed discovery document, not a description of an API programme UCSI does not run. Access to a UCSI application still requires a UCSI-issued account and an application registration inside the tenant; there is no self-serve onboarding.'
kind: authentication
layout: security
method: probed
name: Ucsi Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- deviceCode
overview: UCSI University secures its APIs with oauth2, openIdConnect, and saml2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, and deviceCode flow(s).
provider_name: UCSI University
provider_slug: ucsi
scheme_count: 2
schemes:
- authorization_endpoint: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/oauth2/v2.0/authorize
  device_authorization_endpoint: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/oauth2/v2.0/devicecode
  end_session_endpoint: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/oauth2/v2.0/logout
  federation_brand_name: UCSI University
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/v2.0
  jwks_uri: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/discovery/v2.0/keys
  name: entraOpenIdConnect
  namespace_type: Managed
  openIdConnectUrl: https://login.microsoftonline.com/ucsiuniversity.edu.my/v2.0/.well-known/openid-configuration
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
  sources:
  - https://login.microsoftonline.com/ucsiuniversity.edu.my/v2.0/.well-known/openid-configuration
  - https://login.microsoftonline.com/getuserrealm.srf?login=user@ucsiuniversity.edu.my&json=1
  subject_types_supported:
  - pairwise
  tenant_id: 3c5f2d31-81d8-4455-a2bf-531fbc398144
  tenant_region_scope: AS
  token_endpoint: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/oauth2/v2.0/token
  token_endpoint_auth_methods_supported:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - self_signed_tls_client_auth
  type: openIdConnect
  userinfo_endpoint: https://graph.microsoft.com/oidc/userinfo
- entity_id: https://sts.windows.net/3c5f2d31-81d8-4455-a2bf-531fbc398144/
  metadata_url: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/federationmetadata/2007-06/federationmetadata.xml
  name: entraSaml2
  protocols:
  - urn:oasis:names:tc:SAML:2.0:protocol
  - http://docs.oasis-open.org/wsfed/federation/200706
  role: IDPSSODescriptor
  single_sign_on_service:
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
    location: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/saml2
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
    location: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/saml2
  sources:
  - https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/federationmetadata/2007-06/federationmetadata.xml
  type: saml2
slug: ucsi-authentication
source_filename: ucsi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\nname: UCSI University Identity Authentication\ndescription: >-\n  What can actually be established about how a client authenticates against anything UCSI University\n  operates. UCSI publishes no public API and no developer documentation, so this artifact describes\n  the one authentication surface that is publicly readable: the OpenID Connect / SAML 2.0 metadata of\n  the institution's own Microsoft Entra ID tenant. It is a record of a probed discovery document, not\n  a description of an API programme UCSI does not run. Access to a UCSI application still requires a\n  UCSI-issued account and an application registration inside the tenant; there is no self-serve\n  onboarding.\ngenerated: '2026-09-01'\nmethod: probed\nsource: https://login.microsoftonline.com/ucsiuniversity.edu.my/v2.0/.well-known/openid-configuration\nx-operator: federation\nsummary:\n  types:\n    - oauth2\n    - openIdConnect\n    - saml2\n  oauth2_flows:\n    - authorizationCode\n    - implicit\n \
  \   - deviceCode\nschemes:\n  - name: entraOpenIdConnect\n    type: openIdConnect\n    openIdConnectUrl: https://login.microsoftonline.com/ucsiuniversity.edu.my/v2.0/.well-known/openid-configuration\n    issuer: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/v2.0\n    tenant_id: 3c5f2d31-81d8-4455-a2bf-531fbc398144\n    tenant_region_scope: AS\n    federation_brand_name: UCSI University\n    namespace_type: Managed\n    authorization_endpoint: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/oauth2/v2.0/authorize\n    token_endpoint: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/oauth2/v2.0/token\n    device_authorization_endpoint: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/oauth2/v2.0/devicecode\n    end_session_endpoint: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/oauth2/v2.0/logout\n    userinfo_endpoint: https://graph.microsoft.com/oidc/userinfo\n    jwks_uri:\
  \ https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/discovery/v2.0/keys\n    response_types_supported:\n      - code\n      - id_token\n      - code id_token\n      - id_token token\n    scopes_supported:\n      - openid\n      - profile\n      - email\n      - offline_access\n    token_endpoint_auth_methods_supported:\n      - client_secret_post\n      - client_secret_basic\n      - private_key_jwt\n      - self_signed_tls_client_auth\n    id_token_signing_alg_values_supported:\n      - RS256\n    subject_types_supported:\n      - pairwise\n    sources:\n      - https://login.microsoftonline.com/ucsiuniversity.edu.my/v2.0/.well-known/openid-configuration\n      - https://login.microsoftonline.com/getuserrealm.srf?login=user@ucsiuniversity.edu.my&json=1\n  - name: entraSaml2\n    type: saml2\n    entity_id: https://sts.windows.net/3c5f2d31-81d8-4455-a2bf-531fbc398144/\n    metadata_url: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/federationmetadata/2007-06/federationmetadata.xml\n\
  \    role: IDPSSODescriptor\n    protocols:\n      - urn:oasis:names:tc:SAML:2.0:protocol\n      - http://docs.oasis-open.org/wsfed/federation/200706\n    single_sign_on_service:\n      - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n        location: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/saml2\n      - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n        location: https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/saml2\n    sources:\n      - https://login.microsoftonline.com/3c5f2d31-81d8-4455-a2bf-531fbc398144/federationmetadata/2007-06/federationmetadata.xml\nnotes:\n  - >-\n    The contract behind both schemes is Microsoft's; the TENANT, its branding, its domain and the\n    accounts inside it are UCSI's. Recorded as x-operator federation for that reason.\n  - >-\n    No authentication scheme could be established for koha.ucsiuniversity.edu.my, iis.ucsiuniversity.edu.my\n    or any other institution host:\
  \ Cloudflare returns 403 to automated clients across the estate.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ucsi/refs/heads/main/authentication/ucsi-authentication.yml
summary_line: oauth2/openIdConnect/saml2 · 2 schemes
tags:
- Education
- Higher Education
- University
- Private University
- Malaysia
- Asia
- Library
- Library Catalog
- Koha
- Identity Federation
- Learning Management
- Registry
---
