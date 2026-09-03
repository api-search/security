---
api_key_in: []
auth_types:
- saml2
- openid_connect
- jwt_bearer
- none
description: ''
kind: authentication
layout: security
method: probed
name: Queen Mary University Of London Authentication
name_suffix: Authentication
oauth_flows: []
overview: Queen Mary University of London secures its APIs with saml2, openid_connect, jwt_bearer, and none across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Queen Mary University of London
provider_slug: queen-mary-university-of-london
scheme_count: 5
schemes:
- description: 'Shibboleth Identity Provider for staff, students and federated e-resource access, entityID https://idp.shibboleth.qmul.ac.uk/idp/shibboleth, asserting shibmd:Scope "qmul.ac.uk". Registered in the Jisc UK Access Management Federation and through it eduGAIN. Institutional single sign-on infrastructure, not a developer API: no application can obtain an assertion without being registered as a service provider in the federation.'
  entity_id: https://idp.shibboleth.qmul.ac.uk/idp/shibboleth
  evidence:
  - detail: Signed SAML EntityDescriptor, 9691 bytes, content-type application/samlmetadata+xml, validUntil 2026-09-22. Saved to this repo.
    location: http://mdq.ukfederation.org.uk/entities/https%3A%2F%2Fidp.shibboleth.qmul.ac.uk%2Fidp%2Fshibboleth
    status: 200
  metadata: authentication/queen-mary-university-of-london-saml-idp-metadata.xml
  name: shibboleth-saml2
  protocols:
  - urn:oasis:names:tc:SAML:2.0:protocol
  - urn:oasis:names:tc:SAML:1.1:protocol
  - urn:mace:shibboleth:1.0
  sso_endpoints:
  - https://idp.shibboleth.qmul.ac.uk/idp/profile/SAML2/Redirect/SSO
  - https://idp.shibboleth.qmul.ac.uk/idp/profile/SAML2/POST/SSO
  - https://idp.shibboleth.qmul.ac.uk/idp/profile/Shibboleth/SSO
  type: saml2
  x-operator: federation
- description: Queen Mary's Microsoft Entra ID tenant, GUID 569df091-b013-40e3-86ee-bd9cb9e25814, region scope EU. The OpenID Connect discovery document resolves from the qmul.ac.uk domain hint, which is what proves the tenant belongs to the institution rather than to a supplier. The same tenant GUID appears in the Entra application-proxy CNAME fronting elements.qmul.ac.uk, the university's Symplectic Elements deployment. This is the sign-in plane for institutional applications; it is not an open API and no client can register itself against it.
  discovery: authentication/queen-mary-university-of-london-entra-openid-configuration.json
  evidence:
  - detail: 1964 bytes of JSON. issuer, authorization_endpoint, token_endpoint and jwks_uri all resolve to tenant 569df091-b013-40e3-86ee-bd9cb9e25814. Saved to this repo.
    location: https://login.microsoftonline.com/qmul.ac.uk/v2.0/.well-known/openid-configuration
    status: 200
  - detail: CNAME chain elements-qmulprod.msappproxy.net -> 569df091-b013-40e3-86ee-bd9cb9e25814.tenant.runtime.msappproxy.net, corroborating the tenant GUID from an independent signal.
    location: elements.qmul.ac.uk (DNS)
    status: 200
  issuer: https://login.microsoftonline.com/569df091-b013-40e3-86ee-bd9cb9e25814/v2.0
  name: entra-id-openid-connect
  type: openid_connect
  x-operator: federation
- auth_endpoint: https://qmplus.qmul.ac.uk/mod/lti/auth.php
  description: QMplus, Queen Mary's Moodle learning platform, acts as an LTI 1.3 / LTI Advantage tool platform and publishes its RSA public key set at a stable, unauthenticated URL. Learning tools present a signed JWT to the token endpoint to obtain an access token for the Advantage services. The keys are Queen Mary's own; Moodle is the software, the keypair and the platform issuer are the institution's.
  evidence:
  - detail: 553 bytes application/json. One RSA signing key, kid 320e76b70c41719705ce, alg RS256, use sig. Saved to this repo.
    location: https://qmplus.qmul.ac.uk/mod/lti/certs.php
    status: 200
  - detail: Endpoint present and rejecting a bare GET, which is the protocol's own behaviour, not an outage.
    location: https://qmplus.qmul.ac.uk/mod/lti/token.php
    status: 400
  - detail: application/json 405, endpoint present, method not allowed for GET.
    location: https://qmplus.qmul.ac.uk/mod/lti/services.php
    status: 405
  jwks: authentication/queen-mary-university-of-london-qmplus-lti-jwks.json
  jwks_uri: https://qmplus.qmul.ac.uk/mod/lti/certs.php
  name: lti-1-3-tool-platform
  services_endpoint: https://qmplus.qmul.ac.uk/mod/lti/services.php
  token_endpoint: https://qmplus.qmul.ac.uk/mod/lti/token.php
  type: jwt_bearer
  x-operator: institution
- description: QMplus exposes the standard Moodle web-services REST entry point. It answers unauthenticated with a structured invalidtoken exception, which confirms the endpoint is live and that access is by institutionally issued token only. There is no self-service route to a token.
  evidence:
  - detail: application/xml, EXCEPTION class core\exception\moodle_exception, ERRORCODE invalidtoken, MESSAGE "Invalid token - token not found".
    location: https://qmplus.qmul.ac.uk/webservice/rest/server.php
    status: 200
  location: https://qmplus.qmul.ac.uk/webservice/rest/server.php
  name: moodle-webservice-token
  type: token
  x-operator: institution
- description: The QMRO DSpace 8.4 REST API serves its HAL service document and public repository metadata without a credential. Write and administrative resources sit behind the DSpace authn plane at /server/api/authn.
  location: https://qmro.qmul.ac.uk/server/api
  name: none
  type: none
  x-operator: institution
slug: queen-mary-university-of-london-authentication
source_filename: queen-mary-university-of-london-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live probes on 2026-09-01 of Queen Mary University of London's own authentication surfaces: the\n  institution's signed SAML entity descriptor retrieved from the Jisc UK Access Management\n  Federation MDQ service, the Microsoft Entra ID tenant OpenID Connect discovery document resolved\n  from the qmul.ac.uk domain hint, and the LTI 1.3 Advantage public key set published by the\n  QMplus (Moodle) learning platform.\nx-operator: institution\n\nsummary:\n  note: >-\n    Queen Mary operates no public OAuth authorization server, publishes no developer portal, and\n    issues no self-service API credentials. Its institution-operated authentication is federated\n    identity for people — Shibboleth/SAML into the UK Access Management Federation for\n    inter-organisational access, and a Microsoft Entra ID tenant for cloud and application sign-in\n    — plus an LTI 1.3 tool-platform keyset used to authorise learning-tool\
  \ integrations. The one\n    institution-operated read surface that answers unauthenticated, the QMRO DSpace REST API,\n    requires no credential for public metadata and returns 401 for anything else.\n  types:\n  - saml2\n  - openid_connect\n  - jwt_bearer\n  - none\n  public_oauth: false\n  self_serve_api_keys: false\n\nschemes:\n- name: shibboleth-saml2\n  type: saml2\n  x-operator: federation\n  description: >-\n    Shibboleth Identity Provider for staff, students and federated e-resource access, entityID\n    https://idp.shibboleth.qmul.ac.uk/idp/shibboleth, asserting shibmd:Scope \"qmul.ac.uk\".\n    Registered in the Jisc UK Access Management Federation and through it eduGAIN. Institutional\n    single sign-on infrastructure, not a developer API: no application can obtain an assertion\n    without being registered as a service provider in the federation.\n  metadata: authentication/queen-mary-university-of-london-saml-idp-metadata.xml\n  entity_id: https://idp.shibboleth.qmul.ac.uk/idp/shibboleth\n\
  \  sso_endpoints:\n  - https://idp.shibboleth.qmul.ac.uk/idp/profile/SAML2/Redirect/SSO\n  - https://idp.shibboleth.qmul.ac.uk/idp/profile/SAML2/POST/SSO\n  - https://idp.shibboleth.qmul.ac.uk/idp/profile/Shibboleth/SSO\n  protocols:\n  - urn:oasis:names:tc:SAML:2.0:protocol\n  - urn:oasis:names:tc:SAML:1.1:protocol\n  - urn:mace:shibboleth:1.0\n  evidence:\n  - location: http://mdq.ukfederation.org.uk/entities/https%3A%2F%2Fidp.shibboleth.qmul.ac.uk%2Fidp%2Fshibboleth\n    status: 200\n    detail: >-\n      Signed SAML EntityDescriptor, 9691 bytes, content-type application/samlmetadata+xml,\n      validUntil 2026-09-22. Saved to this repo.\n\n- name: entra-id-openid-connect\n  type: openid_connect\n  x-operator: federation\n  description: >-\n    Queen Mary's Microsoft Entra ID tenant, GUID 569df091-b013-40e3-86ee-bd9cb9e25814, region\n    scope EU. The OpenID Connect discovery document resolves from the qmul.ac.uk domain hint, which\n    is what proves the tenant belongs to the institution\
  \ rather than to a supplier. The same tenant\n    GUID appears in the Entra application-proxy CNAME fronting elements.qmul.ac.uk, the university's\n    Symplectic Elements deployment. This is the sign-in plane for institutional applications; it is\n    not an open API and no client can register itself against it.\n  discovery: authentication/queen-mary-university-of-london-entra-openid-configuration.json\n  issuer: https://login.microsoftonline.com/569df091-b013-40e3-86ee-bd9cb9e25814/v2.0\n  evidence:\n  - location: https://login.microsoftonline.com/qmul.ac.uk/v2.0/.well-known/openid-configuration\n    status: 200\n    detail: >-\n      1964 bytes of JSON. issuer, authorization_endpoint, token_endpoint and jwks_uri all resolve\n      to tenant 569df091-b013-40e3-86ee-bd9cb9e25814. Saved to this repo.\n  - location: elements.qmul.ac.uk (DNS)\n    status: 200\n    detail: >-\n      CNAME chain elements-qmulprod.msappproxy.net ->\n      569df091-b013-40e3-86ee-bd9cb9e25814.tenant.runtime.msappproxy.net,\
  \ corroborating the tenant\n      GUID from an independent signal.\n\n- name: lti-1-3-tool-platform\n  type: jwt_bearer\n  x-operator: institution\n  description: >-\n    QMplus, Queen Mary's Moodle learning platform, acts as an LTI 1.3 / LTI Advantage tool platform\n    and publishes its RSA public key set at a stable, unauthenticated URL. Learning tools present a\n    signed JWT to the token endpoint to obtain an access token for the Advantage services. The keys\n    are Queen Mary's own; Moodle is the software, the keypair and the platform issuer are the\n    institution's.\n  jwks: authentication/queen-mary-university-of-london-qmplus-lti-jwks.json\n  jwks_uri: https://qmplus.qmul.ac.uk/mod/lti/certs.php\n  token_endpoint: https://qmplus.qmul.ac.uk/mod/lti/token.php\n  auth_endpoint: https://qmplus.qmul.ac.uk/mod/lti/auth.php\n  services_endpoint: https://qmplus.qmul.ac.uk/mod/lti/services.php\n  evidence:\n  - location: https://qmplus.qmul.ac.uk/mod/lti/certs.php\n    status: 200\n\
  \    detail: >-\n      553 bytes application/json. One RSA signing key, kid 320e76b70c41719705ce, alg RS256,\n      use sig. Saved to this repo.\n  - location: https://qmplus.qmul.ac.uk/mod/lti/token.php\n    status: 400\n    detail: >-\n      Endpoint present and rejecting a bare GET, which is the protocol's own behaviour, not an\n      outage.\n  - location: https://qmplus.qmul.ac.uk/mod/lti/services.php\n    status: 405\n    detail: application/json 405, endpoint present, method not allowed for GET.\n\n- name: moodle-webservice-token\n  type: token\n  x-operator: institution\n  description: >-\n    QMplus exposes the standard Moodle web-services REST entry point. It answers unauthenticated\n    with a structured invalidtoken exception, which confirms the endpoint is live and that access\n    is by institutionally issued token only. There is no self-service route to a token.\n  location: https://qmplus.qmul.ac.uk/webservice/rest/server.php\n  evidence:\n  - location: https://qmplus.qmul.ac.uk/webservice/rest/server.php\n\
  \    status: 200\n    detail: >-\n      application/xml, EXCEPTION class core\\exception\\moodle_exception, ERRORCODE invalidtoken,\n      MESSAGE \"Invalid token - token not found\".\n\n- name: none\n  type: none\n  x-operator: institution\n  description: >-\n    The QMRO DSpace 8.4 REST API serves its HAL service document and public repository metadata\n    without a credential. Write and administrative resources sit behind the DSpace authn plane at\n    /server/api/authn.\n  location: https://qmro.qmul.ac.uk/server/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/queen-mary-university-of-london/refs/heads/main/authentication/queen-mary-university-of-london-authentication.yml
summary_line: saml2/openid_connect/jwt_bearer/none · 5 schemes
tags:
- University
- Higher Education
- Education
- Research
- United Kingdom
- London
- Russell Group
- Open Access
- Research Repository
- Identity Federation
- Library
- Learning Management
- LTI
- Research Computing
---
