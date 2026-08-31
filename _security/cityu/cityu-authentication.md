---
api_key_in: []
auth_types:
- saml
- oidc
- oauth2
- anonymous
description: ''
kind: authentication
layout: security
method: probed
name: Cityu Authentication
name_suffix: Authentication
oauth_flows: []
overview: City University of Hong Kong secures its APIs with saml, oidc, oauth2, and anonymous across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: City University of Hong Kong
provider_slug: cityu
scheme_count: 4
schemes:
- description: CityUHK's own Shibboleth Identity Provider. Publishes SAML 2.0 + SAML 1.1 IdP metadata at its well-known metadata URL and carries both an IDPSSODescriptor and an AttributeAuthorityDescriptor. Registered in eduGAIN through the Hong Kong Access Federation (registrationAuthority https://hkaf.edu.hk) under the display name "City University of Hong Kong".
  endpoints:
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
    location: https://idp2.cityu.edu.hk/idp/profile/SAML2/Redirect/SSO
    service: SingleSignOnService
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
    location: https://idp2.cityu.edu.hk/idp/profile/SAML2/POST/SSO
    service: SingleSignOnService
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
    location: https://idp2.cityu.edu.hk/idp/profile/SAML2/Redirect/SLO
    service: SingleLogoutService
  - binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP
    location: https://idp2.cityu.edu.hk:8443/idp/profile/SAML2/SOAP/AttributeQuery
    service: AttributeService
  entity_id: https://idp2.cityu.edu.hk/idp/shibboleth
  metadata_file: authentication/cityu-shibboleth-idp-metadata.xml
  metadata_url: https://idp2.cityu.edu.hk/idp/shibboleth
  name: shibboleth-idp
  observations:
  - The shibmd:Scope element in the published metadata still carries the Shibboleth distribution's default value "example.org" rather than cityu.edu.hk. Recorded as observed; not corrected here.
  probed:
  - bytes: 14703
    content_type: application/xml;charset=utf-8
    status: 200
    url: https://idp2.cityu.edu.hk/idp/shibboleth
  protocols:
  - urn:oasis:names:tc:SAML:2.0:protocol
  - urn:oasis:names:tc:SAML:1.1:protocol
  - urn:mace:shibboleth:1.0
  type: saml
  x-operator: institution
- authorization_endpoint: https://auth.cityu.edu.hk/oauth2/v1/authorize
  description: CityUHK's OpenID Connect / OAuth 2.0 authorization server, served on the university's own hostname auth.cityu.edu.hk, which CNAMEs to cityu.customdomains.okta.com. The issuer is https://auth.cityu.edu.hk. This is CityUHK's tenant of Okta, not software CityUHK wrote; the discovery document is the OpenID Connect Discovery 1.0 standard, and the configuration in it is CityUHK's.
  discovery_url: https://auth.cityu.edu.hk/.well-known/openid-configuration
  id_token_signing_alg_values_supported:
  - RS256
  issuer: https://auth.cityu.edu.hk
  jwks_uri: https://auth.cityu.edu.hk/oauth2/v1/keys
  name: cityu-okta-oidc
  oauth_metadata_url: https://auth.cityu.edu.hk/.well-known/oauth-authorization-server
  probed:
  - bytes: 2804
    content_type: application/json
    status: 200
    url: https://auth.cityu.edu.hk/.well-known/openid-configuration
  - bytes: 4165
    content_type: application/json
    status: 200
    url: https://auth.cityu.edu.hk/.well-known/oauth-authorization-server
  - status: 200
    url: https://auth.cityu.edu.hk/oauth2/v1/keys
  scopes_supported:
  - openid
  - email
  - profile
  - address
  - phone
  - offline_access
  - groups
  token_endpoint: https://auth.cityu.edu.hk/oauth2/v1/token
  type: oidc
  userinfo_endpoint: https://auth.cityu.edu.hk/oauth2/v1/userinfo
  x-operator: tenant
- description: SAML 2.0 IdP metadata for the CityUHK Canvas application, served from the university's Okta tenant. Reached by following canvas.cityu.edu.hk, which redirects unauthenticated traffic to auth.cityu.edu.hk with a SAMLRequest.
  entity_id: http://www.okta.com/exk1h9fleyX6q1zrz5d7
  metadata_url: https://auth.cityu.edu.hk/app/exk1h9fleyX6q1zrz5d7/sso/saml/metadata
  name: cityu-okta-saml-canvas
  probed:
  - bytes: 2619
    content_type: application/samlmetadata+xml
    status: 200
    url: https://auth.cityu.edu.hk/app/exk1h9fleyX6q1zrz5d7/sso/saml/metadata
  type: saml
  x-operator: tenant
- description: The CityUHK Scholars OAI-PMH endpoint requires no authentication. The companion Pure REST web service at /ws/api is gated by an api-key header scheme defined in Elsevier's own contract; that contract is not held in this repository.
  name: scholars-oai-anonymous
  probed:
  - content_type: application/xml
    status: 200
    url: https://scholars.cityu.edu.hk/ws/oai?verb=Identify
  type: anonymous
  x-operator: tenant
slug: cityu-authentication
source_filename: cityu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live HTTP probes of CityUHK identity hosts on 2026-08-30, plus the eduGAIN\n  entity database (technical.edugain.org) for the HKAF federation registration.\nnote: >-\n  This file replaces a 2026-07-11 version whose only source was the Elsevier Pure\n  web-service OpenAPI (openapi/cityu-scholars-pure-ws.yaml). That contract is\n  Elsevier's, not CityUHK's, and was removed on 2026-08-30 under the university\n  pipeline's operator-attribution rule. What is recorded here is only what\n  CityUHK itself operates or tenants.\nsummary:\n  types:\n  - saml\n  - oidc\n  - oauth2\n  - anonymous\n  federations:\n  - HKAF (Hong Kong Access Federation, JUCC) — in eduGAIN production since 2018-03-15\n  - eduGAIN\nschemes:\n- name: shibboleth-idp\n  type: saml\n  x-operator: institution\n  description: >-\n    CityUHK's own Shibboleth Identity Provider. Publishes SAML 2.0 + SAML 1.1\n    IdP metadata at its well-known metadata URL\
  \ and carries both an\n    IDPSSODescriptor and an AttributeAuthorityDescriptor. Registered in eduGAIN\n    through the Hong Kong Access Federation (registrationAuthority\n    https://hkaf.edu.hk) under the display name \"City University of Hong Kong\".\n  entity_id: https://idp2.cityu.edu.hk/idp/shibboleth\n  metadata_url: https://idp2.cityu.edu.hk/idp/shibboleth\n  metadata_file: authentication/cityu-shibboleth-idp-metadata.xml\n  protocols:\n  - urn:oasis:names:tc:SAML:2.0:protocol\n  - urn:oasis:names:tc:SAML:1.1:protocol\n  - urn:mace:shibboleth:1.0\n  endpoints:\n  - service: SingleSignOnService\n    binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    location: https://idp2.cityu.edu.hk/idp/profile/SAML2/Redirect/SSO\n  - service: SingleSignOnService\n    binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n    location: https://idp2.cityu.edu.hk/idp/profile/SAML2/POST/SSO\n  - service: SingleLogoutService\n    binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n\
  \    location: https://idp2.cityu.edu.hk/idp/profile/SAML2/Redirect/SLO\n  - service: AttributeService\n    binding: urn:oasis:names:tc:SAML:2.0:bindings:SOAP\n    location: https://idp2.cityu.edu.hk:8443/idp/profile/SAML2/SOAP/AttributeQuery\n  observations:\n  - >-\n    The shibmd:Scope element in the published metadata still carries the\n    Shibboleth distribution's default value \"example.org\" rather than\n    cityu.edu.hk. Recorded as observed; not corrected here.\n  probed:\n  - url: https://idp2.cityu.edu.hk/idp/shibboleth\n    status: 200\n    content_type: application/xml;charset=utf-8\n    bytes: 14703\n- name: cityu-okta-oidc\n  type: oidc\n  x-operator: tenant\n  description: >-\n    CityUHK's OpenID Connect / OAuth 2.0 authorization server, served on the\n    university's own hostname auth.cityu.edu.hk, which CNAMEs to\n    cityu.customdomains.okta.com. The issuer is https://auth.cityu.edu.hk. This\n    is CityUHK's tenant of Okta, not software CityUHK wrote; the discovery\n\
  \    document is the OpenID Connect Discovery 1.0 standard, and the configuration\n    in it is CityUHK's.\n  issuer: https://auth.cityu.edu.hk\n  discovery_url: https://auth.cityu.edu.hk/.well-known/openid-configuration\n  oauth_metadata_url: https://auth.cityu.edu.hk/.well-known/oauth-authorization-server\n  jwks_uri: https://auth.cityu.edu.hk/oauth2/v1/keys\n  authorization_endpoint: https://auth.cityu.edu.hk/oauth2/v1/authorize\n  token_endpoint: https://auth.cityu.edu.hk/oauth2/v1/token\n  userinfo_endpoint: https://auth.cityu.edu.hk/oauth2/v1/userinfo\n  scopes_supported:\n  - openid\n  - email\n  - profile\n  - address\n  - phone\n  - offline_access\n  - groups\n  id_token_signing_alg_values_supported:\n  - RS256\n  probed:\n  - url: https://auth.cityu.edu.hk/.well-known/openid-configuration\n    status: 200\n    content_type: application/json\n    bytes: 2804\n  - url: https://auth.cityu.edu.hk/.well-known/oauth-authorization-server\n    status: 200\n    content_type: application/json\n\
  \    bytes: 4165\n  - url: https://auth.cityu.edu.hk/oauth2/v1/keys\n    status: 200\n- name: cityu-okta-saml-canvas\n  type: saml\n  x-operator: tenant\n  description: >-\n    SAML 2.0 IdP metadata for the CityUHK Canvas application, served from the\n    university's Okta tenant. Reached by following canvas.cityu.edu.hk, which\n    redirects unauthenticated traffic to auth.cityu.edu.hk with a SAMLRequest.\n  metadata_url: https://auth.cityu.edu.hk/app/exk1h9fleyX6q1zrz5d7/sso/saml/metadata\n  entity_id: http://www.okta.com/exk1h9fleyX6q1zrz5d7\n  probed:\n  - url: https://auth.cityu.edu.hk/app/exk1h9fleyX6q1zrz5d7/sso/saml/metadata\n    status: 200\n    content_type: application/samlmetadata+xml\n    bytes: 2619\n- name: scholars-oai-anonymous\n  type: anonymous\n  x-operator: tenant\n  description: >-\n    The CityUHK Scholars OAI-PMH endpoint requires no authentication. The\n    companion Pure REST web service at /ws/api is gated by an api-key header\n    scheme defined in Elsevier's\
  \ own contract; that contract is not held in this\n    repository.\n  probed:\n  - url: https://scholars.cityu.edu.hk/ws/oai?verb=Identify\n    status: 200\n    content_type: application/xml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cityu/refs/heads/main/authentication/cityu-authentication.yml
summary_line: saml/oidc/oauth2/anonymous · 4 schemes
tags:
- Education
- Higher Education
- University
- Hong Kong
- China
- Research
- Institutional Repository
- OAI-PMH
- Identity Federation
- Research Data
- Learning Management
---
