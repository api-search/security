---
api_key_in: []
api_specs:
- filename: ulb-difusion-export-openapi.yml
  format: yaml
  label: DI-fusion Export API
  slug: difusion-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ulb/refs/heads/main/openapi/ulb-difusion-export-openapi.yml
- filename: ulb-difusion-oai-pmh-openapi.yml
  format: yaml
  label: DI-fusion OAI-PMH Harvesting Endpoint
  slug: difusion-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ulb/refs/heads/main/openapi/ulb-difusion-oai-pmh-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Ulb Authentication
name_suffix: Authentication
oauth_flows: []
overview: Université libre de Bruxelles declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Université libre de Bruxelles
provider_slug: ulb
scheme_count: 0
schemes: []
slug: ulb-authentication
source_filename: ulb-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: ULB Authentication Posture\ngenerated: '2026-08-30'\nmethod: probed\nsource: >-\n  Live probes on 2026-08-30 of https://difusion-svc.ulb.ac.be/scholar,\n  https://difusion.ulb.ac.be/vufind/OAI/Server, https://auth.ulb.be/,\n  https://auth.ulb.be/idp/metadata and https://cvchercheurs.ulb.be/.\nx-operator: institution\nsummary: >-\n  ULB's two publicly reachable machine-readable surfaces require no credential at all. Everything\n  else in the ULB estate sits behind a single institutional login at auth.ulb.be, which is a\n  SAML 2.0 identity provider registered in the Belnet R&E Federation and published to eduGAIN.\nsurfaces:\n  - name: DI-fusion Export API\n    base_url: https://difusion-svc.ulb.ac.be\n    scheme: none\n    detail: >-\n      No API key, no token, no session. A bare GET with the two mandatory query parameters returns\n      200 and live bibliographic data. No rate-limit, quota or throttling headers are present on\n      the response; the only headers returned\
  \ are Server: Apache and Content-Type.\n    verified: '2026-08-30'\n  - name: DI-fusion OAI-PMH\n    base_url: https://difusion.ulb.ac.be/vufind/OAI/Server\n    scheme: none\n    detail: Open harvesting endpoint, no credential. Use is governed by the DI-fusion terms of use rather than by an access control.\n    verified: '2026-08-30'\n  - name: ULB Login\n    base_url: https://auth.ulb.be\n    scheme: institutional_sso\n    detail: >-\n      Central ULB login. `https://auth.ulb.be/` redirects to `/login`; the CAS-style paths\n      (/cas/login, /cas/serviceValidate) and the OIDC discovery document return HTTP 403 with a\n      JSON body `{\"status\":403,\"error\":\"Forbidden\",\"message\":\"Access Denied\"}`. No public client\n      registration or OIDC discovery is offered.\n    verified: '2026-08-30'\n  - name: ULB Shibboleth Identity Provider\n    base_url: https://auth.ulb.be/idp\n    scheme: saml2\n    entity_id: https://auth.ulb.be/idp\n    detail: >-\n      SAML 2.0 metadata is\
  \ published unauthenticated at https://auth.ulb.be/idp/metadata (HTTP 200,\n      text/xml, 8,686 bytes). It declares IDPSSODescriptor and AttributeAuthorityDescriptor roles,\n      SingleSignOnService, SingleLogoutService and AttributeService endpoints over HTTP-Redirect,\n      HTTP-POST, HTTP-POST-SimpleSign and SOAP bindings, and a shibmd:Scope of `ulb.be`. It carries\n      the REFEDS Research and Scholarship entity category and the REFEDS SIRTFI assurance\n      certification, registered by http://federation.belnet.be/.\n    verified: '2026-08-30'\n  - name: cvchercheurs.ulb.be\n    base_url: https://cvchercheurs.ulb.be\n    scheme: institutional_sso\n    detail: The researcher CV application, which consumes the DI-fusion export service, is behind ULB Login. Not a public surface.\n    verified: '2026-08-30'\nnotes:\n  - No OAuth 2.0 authorization server, no OIDC discovery document and no developer key issuance exist anywhere on ULB's public estate.\n  - 'https://www.ulb.be/.well-known/security.txt\
  \ returns 404. https://www.ulb.be/llms.txt returns 404.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ulb/refs/heads/main/authentication/ulb-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Belgium
- Europe
- Research
- Research Data
- Institutional Repository
- Open Access
- Identity Federation
- OAI-PMH
- Library
---
