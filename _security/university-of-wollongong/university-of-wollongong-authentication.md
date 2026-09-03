---
api_key_in: []
auth_types:
- saml2
description: ''
kind: authentication
layout: security
method: probed
name: University Of Wollongong Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Wollongong secures its APIs with saml2 across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Wollongong
provider_slug: university-of-wollongong
scheme_count: 1
schemes:
- description: 'entityID https://idp.uow.edu.au/idp/shibboleth, shibmd:Scope uow.edu.au. Bindings: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST at https://idp.uow.edu.au/idp/profile/SAML2/POST/SSO and urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect at https://idp.uow.edu.au/idp/profile/SAML2/Redirect/SSO. NameIDFormat urn:oasis:names:tc:SAML:2.0:nameid-format:transient. Separate IdP-Signing and IdP-Encryption X.509 certificates, both issued 2016-07-27 and valid to 2036-07-27 with subjectAltName idp.uow.edu.au. Requested attributes: auEduPersonSharedToken (urn:oid:1.3.6.1.4.1.27856.1.2.5), email (urn:oid:0.9.2342.19200300.100.1.3) and displayName (urn:oid:2.16.840.1.113730.3.1.241). Organization block declares "The University of Wollongong" at http://www.uow.edu.au/. Runs on AAF''s Rapid IdP managed Shibboleth service.'
  format: SAML 2.0 AuthnRequest / Response
  in: browser
  issuance: 'Not self-service. Trust is established through federation membership, not through a developer signup: a service provider joins the Australian Access Federation, its metadata enters the AAF aggregate at https://md.aaf.edu.au/aaf-metadata.xml, and UOW''s IdP releases attributes to it under AAF policy. There is no public route for an unaffiliated developer to obtain UOW credentials.'
  issued_at: https://idp.uow.edu.au/idp/shibboleth
  name: UOW Shibboleth SAML 2.0 SSO
  parameter: SAMLRequest
  purpose: Federated single sign-on for UOW staff and students into AAF and eduGAIN service providers, and into UOW's own credential-gated systems.
  scoped: false
  sources:
  - https://idp.uow.edu.au/idp/shibboleth
  - https://md.aaf.edu.au/aaf-metadata.xml
  type: saml2
slug: university-of-wollongong-authentication
source_filename: university-of-wollongong-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: probed\nsource: >-\n  https://idp.uow.edu.au/idp/shibboleth (HTTP 200, application/xml) and\n  https://md.aaf.edu.au/aaf-metadata.xml (HTTP 200), plus anonymous probes of\n  courses.uow.edu.au/api, scholars.uow.edu.au/api and api.uow.edu.au\ndocs: https://www.uow.edu.au/its/\nsummary:\n  types:\n  - saml2\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The University of Wollongong publishes no API key, OAuth or token-issuance programme of any\n    kind. Its one publicly documented, machine-readable authentication surface is federated SSO:\n    a Shibboleth SAML 2.0 Identity Provider whose metadata is served openly and is registered in\n    the Australian Access Federation. Everything else UOW itself operates that answers HTTP is\n    credential-gated with no anonymous discovery path — the UOW Handbook's AWS API Gateway\n    returns 403 \"Missing Authentication Token\" on every path, the Symplectic Discovery /api mount\n    returns 403\
  \ \"Access denied\", and api.uow.edu.au (a MuleSoft CloudHub endpoint,\n    v4fkkn.aus-s1.cloudhub.io) does not accept a TCP connection from the public internet at all.\n    No OpenID Connect discovery document is served: both\n    https://idp.uow.edu.au/.well-known/openid-configuration and\n    https://www.uow.edu.au/.well-known/openid-configuration return HTTP 404.\nschemes:\n- name: UOW Shibboleth SAML 2.0 SSO\n  type: saml2\n  in: browser\n  parameter: SAMLRequest\n  format: SAML 2.0 AuthnRequest / Response\n  purpose: >-\n    Federated single sign-on for UOW staff and students into AAF and eduGAIN service providers,\n    and into UOW's own credential-gated systems.\n  description: >-\n    entityID https://idp.uow.edu.au/idp/shibboleth, shibmd:Scope uow.edu.au. Bindings:\n    urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST at\n    https://idp.uow.edu.au/idp/profile/SAML2/POST/SSO and\n    urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect at\n    https://idp.uow.edu.au/idp/profile/SAML2/Redirect/SSO.\
  \ NameIDFormat\n    urn:oasis:names:tc:SAML:2.0:nameid-format:transient. Separate IdP-Signing and IdP-Encryption\n    X.509 certificates, both issued 2016-07-27 and valid to 2036-07-27 with subjectAltName\n    idp.uow.edu.au. Requested attributes: auEduPersonSharedToken\n    (urn:oid:1.3.6.1.4.1.27856.1.2.5), email (urn:oid:0.9.2342.19200300.100.1.3) and displayName\n    (urn:oid:2.16.840.1.113730.3.1.241). Organization block declares \"The University of\n    Wollongong\" at http://www.uow.edu.au/. Runs on AAF's Rapid IdP managed Shibboleth service.\n  issued_at: https://idp.uow.edu.au/idp/shibboleth\n  issuance: >-\n    Not self-service. Trust is established through federation membership, not through a developer\n    signup: a service provider joins the Australian Access Federation, its metadata enters the\n    AAF aggregate at https://md.aaf.edu.au/aaf-metadata.xml, and UOW's IdP releases attributes to\n    it under AAF policy. There is no public route for an unaffiliated developer to\
  \ obtain UOW\n    credentials.\n  scoped: false\n  sources:\n  - https://idp.uow.edu.au/idp/shibboleth\n  - https://md.aaf.edu.au/aaf-metadata.xml\ngated_surfaces:\n- url: https://courses.uow.edu.au/api/\n  status: 403\n  challenge: '{\"message\": \"Missing Authentication Token\"}'\n  note: AWS API Gateway behind the UOW Handbook; no documented credential, no anonymous route.\n- url: https://scholars.uow.edu.au/api/config\n  status: 403\n  challenge: '{\"error\": \"Forbidden\", \"message\": \"Access denied\"}'\n  note: Symplectic Discovery API mount; vendor-operated, UOW tenancy.\n- url: https://api.uow.edu.au/\n  status: 0\n  challenge: TCP connect timeout on 443 and 80\n  note: >-\n    Resolves to MuleSoft CloudHub (v4fkkn.aus-s1.cloudhub.io, 13.210.59.124 / 13.54.241.245 /\n    13.236.171.124). An institution API gateway exists in DNS but is not publicly reachable.\n- url: https://ro.uow.edu.au/\n  status: 202\n  challenge: 'AWS WAF challenge, x-amzn-waf-action: challenge'\n  note:\
  \ Figshare tenancy; the WAF blocks every anonymous path including OAI-PMH.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-wollongong/refs/heads/main/authentication/university-of-wollongong-authentication.yml
summary_line: saml2 · 1 scheme
tags:
- Education
- Higher Education
- University
- Australia
- New South Wales
- Public Research University
- Identity Federation
- Research Repository
- Library
- Course Catalog
- Open Access
- Persistent Identifiers
---
