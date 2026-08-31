---
api_key_in: []
auth_types:
- saml2
- cas
- oauth2
- oidc
description: ''
kind: authentication
layout: security
method: probed
name: Western Authentication
name_suffix: Authentication
oauth_flows: []
overview: Western University secures its APIs with saml2, cas, oauth2, and oidc across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Western University
provider_slug: western
scheme_count: 4
schemes:
- applies_to: https://shibidp.uwo.ca/idp/shibboleth
  cost: free to federated partners
  developer_usable: false
  evidence: 'entityID https://shibidp.uwo.ca/idp/shibboleth present in the CAF signed metadata aggregate with mdui:DisplayName "University of Western Ontario", shibmd:Scope uwo.ca, registrationAuthority http://www.canarie.ca, registrationInstant 2012-01-01T17:18:00Z. Declares the REFEDS Research and Scholarship entity category and the REFEDS Sirtfi assurance certification. Bindings: HTTP-POST, HTTP-POST-SimpleSign, HTTP-Redirect, plus SOAP artifact resolution and attribute query on :8443. Live probe: https://shibidp.uwo.ca/idp/profile/SAML2/Redirect/SSO returns HTTP 400 to a bare GET; https://shibidp.uwo.ca/idp/status returns HTTP 403.'
  issuance: Service-provider registration through the Canadian Access Federation (CANARIE) or by request to Western Technology Services. Not self-serve.
  name: WesternShibbolethIdP
  purpose: Federated single sign-on for Western staff, faculty and students into institutional and third-party research and scholarship services.
  rotation: Key rollover is managed through the federation aggregate; no public schedule.
  scopes: none
  type: saml2
- applies_to: https://ssocas.uwo.ca/cas
  cost: free to affiliated services
  developer_usable: false
  evidence: GET https://ssocas.uwo.ca/cas/login returns HTTP 200 with the Western login form. GET https://ssocas.uwo.ca/cas/p3/serviceValidate returns HTTP 200 with a well-formed CAS 3.0 protocol response — <cas:serviceResponse><cas:authenticationFailure code="INVALID_REQUEST"> — confirming a live, publicly reachable CAS validation endpoint. GET https://ssocas.uwo.ca/cas/actuator returns HTTP 200 with a Spring Boot actuator link document exposing self and health.
  issuance: Service registration by request to Western Technology Services. Not self-serve.
  name: WesternCASProtocol
  purpose: Ticket-based single sign-on for Western web applications.
  rotation: Not documented.
  scopes: none
  type: cas
- applies_to: https://ssocas.uwo.ca/cas/idp/metadata
  caveat: entityID is the stock Apereo CAS placeholder https://cas.example.org/idp. The descriptor is live and correctly scoped to uwo.ca but its entityID was never configured, and it is not the entity registered in the Canadian Access Federation.
  cost: free to affiliated services
  developer_usable: false
  evidence: HTTP 200, 7,167 bytes, EntityDescriptor / IDPSSODescriptor with protocolSupportEnumeration for SAML 2.0, SAML 1.1 and urn:mace:shibboleth:1.0, shibmd:Scope uwo.ca and an X.509 signing certificate CN=ssocas.uwo.ca valid 2025-06-07 to 2045-06-07.
  issuance: Not self-serve.
  name: WesternCASSamlDescriptor
  purpose: SAML 2.0 identity provider descriptor emitted by the CAS server.
  rotation: Certificate valid to 2045-06-07; no rotation policy published.
  scopes: none
  type: saml2
- applies_to: https://ssocas.uwo.ca/cas/oidc
  claimed_but_unverifiable: true
  cost: free to affiliated services
  developer_usable: false
  evidence: 'WTS advertises OIDC in its SSO service catalogue, but the discovery document is not publicly served: GET https://ssocas.uwo.ca/cas/oidc/.well-known/openid-configuration returns HTTP 403 {"status":403,"error":"Forbidden"} and https://ssocas.uwo.ca/cas/oidc/jwks returns HTTP 403. https://ssocas.uwo.ca/.well-known/openid-configuration returns HTTP 404.'
  issuance: Request-based through Western Technology Services.
  name: WesternOIDC
  purpose: OpenID Connect authentication for affiliated Western services.
  rotation: Not documented.
  scopes: not published
  type: oidc
slug: western-authentication
source_filename: western-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: https://wts.uwo.ca/services/o/single-sign-on-sso-saml2-oauth-oidc-cas/index.html\nx-operator: institution\nsummary:\n  types:\n  - saml2\n  - cas\n  - oauth2\n  - oidc\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    Western has one institutional authentication estate and no developer authorization surface\n    at all. Western Technology Services runs two federation servers: an Apereo CAS server at\n    ssocas.uwo.ca that also emits a SAML IdP descriptor and speaks the CAS protocol, and a\n    Shibboleth Identity Provider at shibidp.uwo.ca that is the entity actually registered in\n    the Canadian Access Federation and exported to eduGAIN. Both are end-user login\n    federations. Neither publishes a client-registration path, a token endpoint, a scope\n    catalogue or a consent screen an outside developer could integrate against — WTS documents\n    integration as a request-based process gated behind institutional affiliation.\
  \ OIDC is\n    advertised in the service catalogue but its discovery document is refused (HTTP 403), so\n    no OIDC surface is publicly usable. The two publicly readable data surfaces on this profile\n    (Scholaris and Borealis) are vendor platforms with their own authentication, recorded under\n    their own operators rather than here.\nschemes:\n- name: WesternShibbolethIdP\n  type: saml2\n  applies_to: https://shibidp.uwo.ca/idp/shibboleth\n  issuance: >-\n    Service-provider registration through the Canadian Access Federation (CANARIE) or by\n    request to Western Technology Services. Not self-serve.\n  cost: free to federated partners\n  purpose: >-\n    Federated single sign-on for Western staff, faculty and students into institutional and\n    third-party research and scholarship services.\n  evidence: >-\n    entityID https://shibidp.uwo.ca/idp/shibboleth present in the CAF signed metadata\n    aggregate with mdui:DisplayName \"University of Western Ontario\", shibmd:Scope\
  \ uwo.ca,\n    registrationAuthority http://www.canarie.ca, registrationInstant 2012-01-01T17:18:00Z.\n    Declares the REFEDS Research and Scholarship entity category and the REFEDS Sirtfi\n    assurance certification. Bindings: HTTP-POST, HTTP-POST-SimpleSign, HTTP-Redirect, plus\n    SOAP artifact resolution and attribute query on :8443. Live probe:\n    https://shibidp.uwo.ca/idp/profile/SAML2/Redirect/SSO returns HTTP 400 to a bare GET;\n    https://shibidp.uwo.ca/idp/status returns HTTP 403.\n  rotation: Key rollover is managed through the federation aggregate; no public schedule.\n  scopes: none\n  developer_usable: false\n- name: WesternCASProtocol\n  type: cas\n  applies_to: https://ssocas.uwo.ca/cas\n  issuance: Service registration by request to Western Technology Services. Not self-serve.\n  cost: free to affiliated services\n  purpose: Ticket-based single sign-on for Western web applications.\n  evidence: >-\n    GET https://ssocas.uwo.ca/cas/login returns HTTP 200 with the\
  \ Western login form. GET\n    https://ssocas.uwo.ca/cas/p3/serviceValidate returns HTTP 200 with a well-formed CAS 3.0\n    protocol response — <cas:serviceResponse><cas:authenticationFailure code=\"INVALID_REQUEST\">\n    — confirming a live, publicly reachable CAS validation endpoint. GET\n    https://ssocas.uwo.ca/cas/actuator returns HTTP 200 with a Spring Boot actuator link\n    document exposing self and health.\n  rotation: Not documented.\n  scopes: none\n  developer_usable: false\n- name: WesternCASSamlDescriptor\n  type: saml2\n  applies_to: https://ssocas.uwo.ca/cas/idp/metadata\n  issuance: Not self-serve.\n  cost: free to affiliated services\n  purpose: SAML 2.0 identity provider descriptor emitted by the CAS server.\n  evidence: >-\n    HTTP 200, 7,167 bytes, EntityDescriptor / IDPSSODescriptor with\n    protocolSupportEnumeration for SAML 2.0, SAML 1.1 and urn:mace:shibboleth:1.0,\n    shibmd:Scope uwo.ca and an X.509 signing certificate CN=ssocas.uwo.ca valid\n    2025-06-07\
  \ to 2045-06-07.\n  rotation: Certificate valid to 2045-06-07; no rotation policy published.\n  scopes: none\n  developer_usable: false\n  caveat: >-\n    entityID is the stock Apereo CAS placeholder https://cas.example.org/idp. The descriptor is\n    live and correctly scoped to uwo.ca but its entityID was never configured, and it is not\n    the entity registered in the Canadian Access Federation.\n- name: WesternOIDC\n  type: oidc\n  applies_to: https://ssocas.uwo.ca/cas/oidc\n  issuance: Request-based through Western Technology Services.\n  cost: free to affiliated services\n  purpose: OpenID Connect authentication for affiliated Western services.\n  evidence: >-\n    WTS advertises OIDC in its SSO service catalogue, but the discovery document is not\n    publicly served: GET https://ssocas.uwo.ca/cas/oidc/.well-known/openid-configuration\n    returns HTTP 403 {\"status\":403,\"error\":\"Forbidden\"} and\n    https://ssocas.uwo.ca/cas/oidc/jwks returns HTTP 403.\n    https://ssocas.uwo.ca/.well-known/openid-configuration\
  \ returns HTTP 404.\n  rotation: Not documented.\n  scopes: not published\n  developer_usable: false\n  claimed_but_unverifiable: true\nnegative_probes:\n- url: https://ssocas.uwo.ca/cas/oidc/.well-known/openid-configuration\n  status: 403\n  note: OIDC discovery refused; advertised capability, no public metadata.\n- url: https://ssocas.uwo.ca/cas/oidc/jwks\n  status: 403\n  note: JWKS refused.\n- url: https://ssocas.uwo.ca/.well-known/openid-configuration\n  status: 404\n- url: https://ssocas.uwo.ca/idp/shibboleth\n  status: 404\n  note: The Shibboleth entityID path is not on the CAS host; the real IdP is shibidp.uwo.ca.\n- url: https://shibidp.uwo.ca/idp/shibboleth\n  status: 404\n  note: >-\n    Metadata is published through the CAF aggregate rather than at the entityID URL. Normal\n    Shibboleth behaviour — the entityID is an identifier, not a required document location.\n- url: https://www.uwo.ca/.well-known/security.txt\n  status: 404\n- url: https://www.uwo.ca/llms.txt\n  status:\
  \ 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/western/refs/heads/main/authentication/western-authentication.yml
summary_line: saml2/cas/oauth2/oidc · 4 schemes
tags:
- University
- Higher Education
- Education
- Research
- Canada
- Ontario
- U15
- Identity Federation
- Research Repository
- Research Data
- Open Access
- OAI-PMH
- Library
---
