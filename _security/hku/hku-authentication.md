---
api_key_in: []
api_specs:
- filename: hku-identity-openapi.yml
  format: yaml
  label: HKU AD FS OAuth 2.0 / OpenID Connect Issuer
  slug: adfs-oidc
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/openapi/hku-identity-openapi.yml
auth_types:
- oauth2
- openIdConnect
- saml2
- apiKey
description: ''
kind: authentication
layout: security
method: probed
name: Hku Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Hong Kong secures its APIs with oauth2, openIdConnect, saml2, and apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Hong Kong
provider_slug: hku
scheme_count: 4
schemes:
- clientAuthentication:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  - windows_client_authentication
  description: HKU-operated AD FS OpenID Connect issuer. RS256 id_tokens, pairwise subject identifiers, JWKS at https://adfs.hku.hk/adfs/discovery/keys.
  flows:
  - authorizationUrl: https://adfs.hku.hk/adfs/oauth2/authorize/
    flow: authorizationCode
    tokenUrl: https://adfs.hku.hk/adfs/oauth2/token/
  - flow: clientCredentials
    tokenUrl: https://adfs.hku.hk/adfs/oauth2/token/
  - deviceAuthorizationUrl: https://adfs.hku.hk/adfs/oauth2/devicecode
    flow: deviceCode
    tokenUrl: https://adfs.hku.hk/adfs/oauth2/token/
  issuer: https://adfs.hku.hk/adfs
  name: hku-adfs-oidc
  openIdConnectUrl: https://adfs.hku.hk/adfs/.well-known/openid-configuration
  registration: private
  registrationNote: No public dynamic client registration; relying parties are registered by HKU ITS.
  sources:
  - well-known/hku-adfs-openid-configuration.json
  type: openIdConnect
- description: Signed WS-Federation / SAML 2.0 federation metadata for the HKU AD FS deployment (200, application/samlmetadata+xml, 71,026 bytes on 2026-08-19).
  entityId: http://adfs.hku.hk/adfs/services/trust
  metadata: https://adfs.hku.hk/FederationMetadata/2007-06/FederationMetadata.xml
  name: hku-adfs-wsfed-saml
  sources:
  - https://adfs.hku.hk/FederationMetadata/2007-06/FederationMetadata.xml
  type: saml2
- assuranceCertification:
  - https://refeds.org/sirtfi
  bindings:
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
  - urn:oasis:names:tc:SAML:2.0:bindings:SOAP
  description: Shibboleth identity provider operated by HKU, self-publishing its metadata (200, application/xml, 14,831 bytes) and present in the eduGAIN interfederation aggregate. Technical and REFEDS security contacts are published in the metadata; they are named individuals and are deliberately not copied into this catalog.
  entityCategories:
  - http://refeds.org/category/research-and-scholarship
  entityId: https://hkafidp.hku.hk/idp/shibboleth
  federation: Hong Kong Access Federation (HKAF, JUCC) — exported to eduGAIN
  metadata: https://hkafidp.hku.hk/idp/shibboleth
  name: hku-shibboleth-idp
  nameIdFormats:
  - urn:oasis:names:tc:SAML:2.0:nameid-format:transient
  registrationAuthority: https://hkaf.edu.hk
  registrationInstant: '2016-12-15T07:04:40Z'
  scope: hku.hk
  sources:
  - https://hkafidp.hku.hk/idp/shibboleth
  - https://mds.edugain.org/edugain-v2.xml
  type: saml2
- audience: HKU staff and students
  description: Azure API Management subscription key pair issued through developer.hku.hk after HKU institutional sign-in, used for the HKU GenAI chat-completion, embedding and image-generation APIs. The portal returns HTTP 200 but redirects every route to /signin, so the API catalog, the header name and the key policy are not publicly readable.
  gated: true
  in: header
  name: hku-its-api-subscription-key
  sources:
  - https://developer.hku.hk/
  type: apiKey
slug: hku-authentication
source_filename: hku-authentication.yml
source_heading: Authentication Profile
source_url: https://adfs.hku.hk/adfs/.well-known/openid-configuration
source_yaml: "generated: '2026-08-19'\nmethod: probed\nsource: https://adfs.hku.hk/adfs/.well-known/openid-configuration\nsources:\n- https://adfs.hku.hk/adfs/.well-known/openid-configuration\n- https://adfs.hku.hk/adfs/discovery/keys\n- https://adfs.hku.hk/FederationMetadata/2007-06/FederationMetadata.xml\n- https://hkafidp.hku.hk/idp/shibboleth\n- https://developer.hku.hk/\nx-operator: institution\nnote: >-\n  Read from live documents on HKU's own hosts on 2026-08-19, not from prose. The University of\n  Hong Kong operates two institution-run authentication surfaces — an AD FS OAuth 2.0 / OpenID\n  Connect issuer at adfs.hku.hk and a Shibboleth SAML 2.0 identity provider at hkafidp.hku.hk\n  registered in eduGAIN through the Hong Kong Access Federation — plus an Azure API Management\n  developer portal at developer.hku.hk whose API keys are issued only to HKU staff and students\n  after institutional sign-in. There is no anonymous, self-serve credential path for anyone\n  outside the University.\n\
  summary:\n  types:\n  - oauth2\n  - openIdConnect\n  - saml2\n  - apiKey\nschemes:\n- name: hku-adfs-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://adfs.hku.hk/adfs/.well-known/openid-configuration\n  issuer: https://adfs.hku.hk/adfs\n  description: >-\n    HKU-operated AD FS OpenID Connect issuer. RS256 id_tokens, pairwise subject identifiers,\n    JWKS at https://adfs.hku.hk/adfs/discovery/keys.\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://adfs.hku.hk/adfs/oauth2/authorize/\n    tokenUrl: https://adfs.hku.hk/adfs/oauth2/token/\n  - flow: clientCredentials\n    tokenUrl: https://adfs.hku.hk/adfs/oauth2/token/\n  - flow: deviceCode\n    deviceAuthorizationUrl: https://adfs.hku.hk/adfs/oauth2/devicecode\n    tokenUrl: https://adfs.hku.hk/adfs/oauth2/token/\n  clientAuthentication:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  - windows_client_authentication\n  registration: private\n  registrationNote: No public dynamic client\
  \ registration; relying parties are registered by HKU ITS.\n  sources:\n  - well-known/hku-adfs-openid-configuration.json\n- name: hku-adfs-wsfed-saml\n  type: saml2\n  entityId: http://adfs.hku.hk/adfs/services/trust\n  metadata: https://adfs.hku.hk/FederationMetadata/2007-06/FederationMetadata.xml\n  description: >-\n    Signed WS-Federation / SAML 2.0 federation metadata for the HKU AD FS deployment\n    (200, application/samlmetadata+xml, 71,026 bytes on 2026-08-19).\n  sources:\n  - https://adfs.hku.hk/FederationMetadata/2007-06/FederationMetadata.xml\n- name: hku-shibboleth-idp\n  type: saml2\n  entityId: https://hkafidp.hku.hk/idp/shibboleth\n  metadata: https://hkafidp.hku.hk/idp/shibboleth\n  scope: hku.hk\n  federation: Hong Kong Access Federation (HKAF, JUCC) — exported to eduGAIN\n  registrationAuthority: https://hkaf.edu.hk\n  registrationInstant: '2016-12-15T07:04:40Z'\n  entityCategories:\n  - http://refeds.org/category/research-and-scholarship\n  assuranceCertification:\n\
  \  - https://refeds.org/sirtfi\n  bindings:\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n  - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n  - urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n  nameIdFormats:\n  - urn:oasis:names:tc:SAML:2.0:nameid-format:transient\n  description: >-\n    Shibboleth identity provider operated by HKU, self-publishing its metadata (200,\n    application/xml, 14,831 bytes) and present in the eduGAIN interfederation aggregate.\n    Technical and REFEDS security contacts are published in the metadata; they are named\n    individuals and are deliberately not copied into this catalog.\n  sources:\n  - https://hkafidp.hku.hk/idp/shibboleth\n  - https://mds.edugain.org/edugain-v2.xml\n- name: hku-its-api-subscription-key\n  type: apiKey\n  in: header\n  description: >-\n    Azure API Management subscription key pair issued through developer.hku.hk after HKU\n    institutional sign-in, used for the HKU GenAI chat-completion, embedding and image-generation\n\
  \    APIs. The portal returns HTTP 200 but redirects every route to /signin, so the API catalog,\n    the header name and the key policy are not publicly readable.\n  gated: true\n  audience: HKU staff and students\n  sources:\n  - https://developer.hku.hk/\ntenantSchemes:\n- name: microsoft-entra-hku-tenant\n  x-operator: tenant\n  type: openIdConnect\n  openIdConnectUrl: https://login.microsoftonline.com/hku.hk/v2.0/.well-known/openid-configuration\n  tenantId: 42f9b54e-2477-41ba-bf09-7a0d2a83ff09\n  description: >-\n    HKU's Microsoft Entra ID tenant. Machine-readable and institution-specific, but operated by\n    Microsoft on Microsoft's host — recorded as a tenant relationship, not as an HKU contract.\n    Microsoft's realm discovery reports domain hku.hk as Federated to https://adfs.hku.hk/adfs/ls/\n    under the brand \"The University Of Hong Kong\".\n  sources:\n  - https://login.microsoftonline.com/hku.hk/v2.0/.well-known/openid-configuration\n  - https://login.microsoftonline.com/getuserrealm.srf?login=user@hku.hk&json=1\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hku/refs/heads/main/authentication/hku-authentication.yml
summary_line: oauth2/openIdConnect/saml2/apiKey · 4 schemes
tags:
- Education
- Higher Education
- University
- Hong Kong
- Identity Federation
- Single Sign-On
- Research Data
- Open Access
- Artificial Intelligence
- Research Computing
---
