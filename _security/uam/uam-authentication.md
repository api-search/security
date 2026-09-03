---
api_key_in: []
auth_types: []
description: 'Authentication posture across every Universidad Autonoma de Madrid surface reachable from the open internet. UAM''s pattern is the opposite of the common one in this cohort: its machine-readable surfaces are anonymously readable, and the gated surfaces publish no machine-readable contract at all. There is no developer program, no API key issuance, no OAuth client registration and no self-service onboarding anywhere in the estate. An unaffiliated caller can harvest the repository and the journals portal today without credentials; everything beyond read access is bound to institutional identity through Shibboleth, and institutional identity is only issued to members of the university.'
kind: authentication
layout: security
method: probed
name: Uam Authentication
name_suffix: Authentication
oauth_flows: []
overview: Autonomous University of Madrid declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Autonomous University of Madrid
provider_slug: uam
scheme_count: 6
schemes:
- applies_to:
  - https://repositorio.uam.es/server/api
  - https://repositorio.uam.es/server/oai/request
  - https://repositorio.uam.es/server/opensearch/service
  - https://revistas.uam.es/index.php/index/oai
  name: Anonymous read (institutional repository and journals portal)
  note: This is the whole of UAM's publicly consumable API surface, and it is real. No key, no registration, no terms acceptance.
  observed: All five endpoints return full payloads to an unauthenticated client. The DSpace REST API sets a DSPACE-XSRF-COOKIE and requires the paired DSPACE-XSRF-TOKEN header for state-changing requests, but read operations need nothing.
  rate_limit_observed: none
  type: none
  x-access: public
  x-operator: institution
- challenge_status: 200
  challenge_url: https://repositorio.uam.es/server/api/authn/status
  discovery_feed: https://repositorio.uam.es/Shibboleth.sso/DiscoFeed
  idp_offered:
  - IDP_UAM
  methods_advertised:
  - shibboleth
  - ip
  - password
  name: Shibboleth / SAML 2.0 (Biblos-e Archivo REST API)
  onboarding: Write access to Biblos-e Archivo requires a UAM institutional account asserted through Shibboleth, or a password account created by the repository administrators. There is no external registration path.
  self_service: false
  sp_entity_id: https://repositorio.uam.es/shibboleth
  sp_metadata: https://repositorio.uam.es/Shibboleth.sso/Metadata
  type: saml
  www_authenticate: shibboleth realm="DSpace REST API", location="https://repositorio.uam.es/Shibboleth.sso/Login?target=https%3A%2F%2Frepositorio.uam.es%2Fserver%2Fapi%2Fauthn%2Fshibboleth", ip realm="DSpace REST API", password realm="DSpace REST API"
  x-access: gated
  x-operator: institution
- detail: identity-federation/uam-identity-federation.yml
  entity_categories:
  - http://refeds.org/category/research-and-scholarship
  entity_id: https://www.rediris.es/sir/uamidp
  name: UAM federated identity in SIR / eduGAIN
  note: The identity is UAM's; the IdP endpoints and the metadata are operated for UAM by RedIRIS inside Spain's national R&E federation. Recorded, never deleted.
  scope: uam.es
  sirtfi: true
  slo_endpoint: https://sir.rediris.es/uam/saml2/idp/SingleLogoutService.php
  sso_endpoint: https://sir.rediris.es/uam/saml2/idp/SSOService.php
  type: saml
  x-access: gated
  x-operator: federation
- authorization_endpoint: https://moodle.uam.es/mod/lti/auth.php
  jwks_uri: https://moodle.uam.es/mod/lti/certs.php
  name: LTI 1.3 / LTI Advantage platform (Moodle)
  onboarding: An LTI tool exists only if a UAM Moodle administrator registers it and issues a client_id and deployment_id. There is no dynamic registration endpoint and no public tool catalogue.
  second_instance_jwks: https://posgrado.uam.es/mod/lti/certs.php
  self_service: false
  signing_algorithms:
  - RS256
  subtype: client_credentials with private_key_jwt (IMS Security Framework)
  token_endpoint: https://moodle.uam.es/mod/lti/token.php
  token_endpoint_probe: POST -> 400 {"error":"invalid_request"}
  type: oauth2
  x-access: gated
  x-operator: institution
- endpoint: https://moodle.uam.es/webservice/rest/server.php
  in: query
  name: Moodle Web Services (REST)
  onboarding: The web services subsystem is enabled and answering, which is a real finding - most institutional Moodles return a disabled-service error instead. Tokens are issued only to accounts a UAM administrator has authorised for a named external service.
  parameter_name: wstoken
  probe_body: <EXCEPTION class="core\exception\moodle_exception"><ERRORCODE>invalidtoken</ERRORCODE> <MESSAGE>Ficha (token) no valida - ficha no encontrada</MESSAGE></EXCEPTION>
  probe_status: 200
  self_service: false
  type: apiKey
  x-access: gated
  x-operator: institution
- checked:
  - path: /idp/shibboleth
    status: 404
  - path: /simplesaml/saml2/idp/metadata.php
    status: 404
  - path: /Shibboleth.sso/Metadata
    status: 404
  - path: /idp/profile/Metadata/SAML
    status: 404
  machine_readable_metadata: none
  name: ID-UAM single sign-on
  note: ID-UAM is the university's account and sign-on service for students and staff. It is live but publishes no OIDC discovery document and no SAML metadata at any conventional path, so it is catalogued as a sign-on surface rather than as an API.
  status: 200
  type: proprietary
  url: https://id.uam.es/
  x-access: gated
  x-operator: institution
slug: uam-authentication
source_filename: uam-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Evangelist Authentication\nspecificationVersion: '0.1'\nprovider: Autonomous University of Madrid\nproviderId: uam\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  https://repositorio.uam.es/server/api/authn/status (200, WWW-Authenticate header captured),\n  https://repositorio.uam.es/server/api (200, anonymous read),\n  https://repositorio.uam.es/Shibboleth.sso/Metadata (200),\n  https://repositorio.uam.es/Shibboleth.sso/DiscoFeed (200),\n  https://repositorio.uam.es/server/oai/request?verb=Identify (200, anonymous),\n  https://revistas.uam.es/index.php/index/oai?verb=Identify (200, anonymous, plain UA),\n  https://moodle.uam.es/webservice/rest/server.php (200, Moodle invalidtoken exception),\n  https://moodle.uam.es/mod/lti/token.php (400 invalid_request, POST),\n  https://moodle.uam.es/mod/lti/certs.php (200), https://id.uam.es/ (200 HTML) and four\n  metadata paths under id.uam.es (all 404). All fetched 2026-09-01.\ndescription: >-\n  Authentication\
  \ posture across every Universidad Autonoma de Madrid surface reachable from the\n  open internet. UAM's pattern is the opposite of the common one in this cohort: its\n  machine-readable surfaces are anonymously readable, and the gated surfaces publish no\n  machine-readable contract at all. There is no developer program, no API key issuance, no\n  OAuth client registration and no self-service onboarding anywhere in the estate. An\n  unaffiliated caller can harvest the repository and the journals portal today without\n  credentials; everything beyond read access is bound to institutional identity through\n  Shibboleth, and institutional identity is only issued to members of the university.\n\nschemes:\n- name: Anonymous read (institutional repository and journals portal)\n  type: none\n  x-operator: institution\n  x-access: public\n  applies_to:\n  - https://repositorio.uam.es/server/api\n  - https://repositorio.uam.es/server/oai/request\n  - https://repositorio.uam.es/server/opensearch/service\n\
  \  - https://revistas.uam.es/index.php/index/oai\n  observed: >-\n    All five endpoints return full payloads to an unauthenticated client. The DSpace REST API\n    sets a DSPACE-XSRF-COOKIE and requires the paired DSPACE-XSRF-TOKEN header for state-changing\n    requests, but read operations need nothing.\n  rate_limit_observed: none\n  note: >-\n    This is the whole of UAM's publicly consumable API surface, and it is real. No key, no\n    registration, no terms acceptance.\n\n- name: Shibboleth / SAML 2.0 (Biblos-e Archivo REST API)\n  type: saml\n  x-operator: institution\n  x-access: gated\n  challenge_url: https://repositorio.uam.es/server/api/authn/status\n  challenge_status: 200\n  www_authenticate: >-\n    shibboleth realm=\"DSpace REST API\",\n    location=\"https://repositorio.uam.es/Shibboleth.sso/Login?target=https%3A%2F%2Frepositorio.uam.es%2Fserver%2Fapi%2Fauthn%2Fshibboleth\",\n    ip realm=\"DSpace REST API\", password realm=\"DSpace REST API\"\n  methods_advertised:\n\
  \  - shibboleth\n  - ip\n  - password\n  sp_entity_id: https://repositorio.uam.es/shibboleth\n  sp_metadata: https://repositorio.uam.es/Shibboleth.sso/Metadata\n  discovery_feed: https://repositorio.uam.es/Shibboleth.sso/DiscoFeed\n  idp_offered:\n  - IDP_UAM\n  self_service: false\n  onboarding: >-\n    Write access to Biblos-e Archivo requires a UAM institutional account asserted through\n    Shibboleth, or a password account created by the repository administrators. There is no\n    external registration path.\n\n- name: UAM federated identity in SIR / eduGAIN\n  type: saml\n  x-operator: federation\n  x-access: gated\n  entity_id: https://www.rediris.es/sir/uamidp\n  sso_endpoint: https://sir.rediris.es/uam/saml2/idp/SSOService.php\n  slo_endpoint: https://sir.rediris.es/uam/saml2/idp/SingleLogoutService.php\n  scope: uam.es\n  sirtfi: true\n  entity_categories:\n  - http://refeds.org/category/research-and-scholarship\n  detail: identity-federation/uam-identity-federation.yml\n  note:\
  \ >-\n    The identity is UAM's; the IdP endpoints and the metadata are operated for UAM by RedIRIS\n    inside Spain's national R&E federation. Recorded, never deleted.\n\n- name: LTI 1.3 / LTI Advantage platform (Moodle)\n  type: oauth2\n  subtype: 'client_credentials with private_key_jwt (IMS Security Framework)'\n  x-operator: institution\n  x-access: gated\n  jwks_uri: https://moodle.uam.es/mod/lti/certs.php\n  authorization_endpoint: https://moodle.uam.es/mod/lti/auth.php\n  token_endpoint: https://moodle.uam.es/mod/lti/token.php\n  token_endpoint_probe: 'POST -> 400 {\"error\":\"invalid_request\"}'\n  second_instance_jwks: https://posgrado.uam.es/mod/lti/certs.php\n  signing_algorithms:\n  - RS256\n  self_service: false\n  onboarding: >-\n    An LTI tool exists only if a UAM Moodle administrator registers it and issues a client_id\n    and deployment_id. There is no dynamic registration endpoint and no public tool catalogue.\n\n- name: Moodle Web Services (REST)\n  type: apiKey\n\
  \  in: query\n  parameter_name: wstoken\n  x-operator: institution\n  x-access: gated\n  endpoint: https://moodle.uam.es/webservice/rest/server.php\n  probe_status: 200\n  probe_body: >-\n    <EXCEPTION class=\"core\\exception\\moodle_exception\"><ERRORCODE>invalidtoken</ERRORCODE>\n    <MESSAGE>Ficha (token) no valida - ficha no encontrada</MESSAGE></EXCEPTION>\n  self_service: false\n  onboarding: >-\n    The web services subsystem is enabled and answering, which is a real finding - most\n    institutional Moodles return a disabled-service error instead. Tokens are issued only to\n    accounts a UAM administrator has authorised for a named external service.\n\n- name: ID-UAM single sign-on\n  type: proprietary\n  x-operator: institution\n  x-access: gated\n  url: https://id.uam.es/\n  status: 200\n  machine_readable_metadata: none\n  checked:\n  - path: /idp/shibboleth\n    status: 404\n  - path: /simplesaml/saml2/idp/metadata.php\n    status: 404\n  - path: /Shibboleth.sso/Metadata\n\
  \    status: 404\n  - path: /idp/profile/Metadata/SAML\n    status: 404\n  note: >-\n    ID-UAM is the university's account and sign-on service for students and staff. It is live\n    but publishes no OIDC discovery document and no SAML metadata at any conventional path, so\n    it is catalogued as a sign-on surface rather than as an API.\n\ndeveloper_program:\n  exists: false\n  portal: none\n  key_issuance: none\n  terms_of_service: not published for any API surface\n  note: >-\n    No developer portal, no API terms, no key or client registration exists anywhere on the\n    uam.es estate. The public surfaces need no credential and the credentialled surfaces are\n    reachable only through institutional identity.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uam/refs/heads/main/authentication/uam-authentication.yml
summary_line: 6 schemes
tags:
- University
- Higher Education
- Education
- Spain
- Public Research University
- Institutional Repository
- Research Data
- Open Access
- OAI-PMH
- Identity Federation
- Learning Management
- DSpace
- Open Journal Systems
- Shibboleth
---
