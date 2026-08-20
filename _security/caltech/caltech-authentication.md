---
api_key_in: []
api_specs:
- filename: caltech-caltechdata-openapi.yml
  format: yaml
  label: CaltechDATA REST API
  slug: caltechdata-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caltech/refs/heads/main/openapi/caltech-caltechdata-openapi.yml
- filename: caltech-scedc-fdsn-openapi.yml
  format: yaml
  label: SCEDC FDSN Web Services
  slug: scedc-fdsn
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caltech/refs/heads/main/openapi/caltech-scedc-fdsn-openapi.yml
auth_types: []
description: Caltech's public machine-readable surfaces are open research infrastructure and require no credential to read. The institution's authentication engineering is concentrated in its identity federation, which is itself a machine-readable surface but governs access to internal systems rather than to the public APIs.
kind: authentication
layout: security
method: probed
name: Caltech Authentication
name_suffix: Authentication
oauth_flows: []
overview: California Institute of Technology declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: California Institute of Technology
provider_slug: caltech
scheme_count: 0
schemes: []
slug: caltech-authentication
source_filename: caltech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "---\naid: caltech\nname: California Institute of Technology — Authentication Posture\ngenerated: '2026-08-19'\nmethod: probed\nsource:\n  - https://data.caltech.edu/api/records?size=1\n  - https://service.scedc.caltech.edu/fdsnws/station/1/version\n  - https://irsa.ipac.caltech.edu/TAP/capabilities\n  - https://idp.caltech.edu/idp/shibboleth\n  - https://mdq.incommon.org/entities/https%3A%2F%2Fidp.caltech.edu%2Fidp%2Fshibboleth\ndescription: >-\n  Caltech's public machine-readable surfaces are open research infrastructure and require\n  no credential to read. The institution's authentication engineering is concentrated in\n  its identity federation, which is itself a machine-readable surface but governs access\n  to internal systems rather than to the public APIs.\n\nsurfaces:\n  - surface: CaltechDATA REST API\n    baseURL: https://data.caltech.edu/api\n    x-operator: institution\n    public_read: true\n    auth_required_for_read: false\n    verified: '2026-08-19 — 200 application/json\
  \ with no Authorization header'\n    write_auth:\n      scheme: bearer\n      type: personal access token\n      note: >-\n        InvenioRDM issues personal access tokens for deposit/write operations. Token\n        issuance is behind authentication and was NOT probed; recorded as software\n        capability, not as a verified Caltech-published contract.\n      method: derived\n\n  - surface: CaltechDATA OAI-PMH\n    baseURL: https://data.caltech.edu/oai2d\n    x-operator: institution\n    public_read: true\n    auth_required_for_read: false\n    verified: '2026-08-19 — Identify verb returned 200 text/xml unauthenticated'\n\n  - surface: CaltechAUTHORS REST + OAI-PMH\n    baseURL: https://authors.library.caltech.edu\n    x-operator: institution\n    public_read: true\n    auth_required_for_read: false\n    verified: '2026-08-19 — 200 application/json unauthenticated'\n    reliability_note: >-\n      Intermittent HTTP 522 (Cloudflare origin unreachable) observed on 2026-08-19\n      between\
  \ successful calls. The surface is LIVE but flapping.\n\n  - surface: SCEDC FDSN Web Services\n    baseURL: https://service.scedc.caltech.edu/fdsnws\n    x-operator: institution\n    public_read: true\n    auth_required_for_read: false\n    verified: '2026-08-19 — real event and station queries returned data unauthenticated'\n    note: >-\n      The FDSN specification defines an optional /queryauth endpoint for restricted data.\n      Not probed; not claimed.\n\n  - surface: IRSA / NED / NASA Exoplanet Archive IVOA services\n    baseURL: https://irsa.ipac.caltech.edu/TAP\n    x-operator: institution\n    public_read: true\n    auth_required_for_read: false\n    verified: '2026-08-19 — TAP sync queries returned real rows unauthenticated'\n    declared_security:\n      standardID: 'ivo://ivoa.net/sso#cookie'\n      source: https://irsa.ipac.caltech.edu/TAP/capabilities\n      note: >-\n        The TAP capabilities document declares an IVOA SSO cookie security method for\n        authenticated\
  \ access to proprietary data. Read as declared in-contract, not probed.\n\n  - surface: Caltech Library Feeds\n    baseURL: https://feeds.library.caltech.edu\n    x-operator: institution\n    public_read: true\n    auth_required_for_read: false\n    verified: '2026-08-19 — JSON datasets returned 200 unauthenticated'\n\nidentity_federation:\n  surface: Caltech Shibboleth Identity Provider\n  entityID: https://idp.caltech.edu/idp/shibboleth\n  x-operator: institution\n  protocols:\n    - urn:mace:shibboleth:1.0\n    - urn:oasis:names:tc:SAML:1.1:protocol\n    - urn:oasis:names:tc:SAML:2.0:protocol\n  scope: caltech.edu\n  federation: InCommon (registrationAuthority https://incommon.org), and therefore eduGAIN\n  sso_bindings:\n    - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n    - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n  attribute_authority: https://idp.caltech.edu:8443/idp/profile/SAML2/SOAP/AttributeQuery\n\
  \  single_logout: https://idp.caltech.edu/idp/profile/Logout\n  verified: '2026-08-19 — metadata retrieved 200 from both the IdP and the InCommon MDQ service'\n  note: >-\n    This governs access to Caltech systems for Caltech identities and for federated\n    partners. It is not an API gateway for the public data surfaces above, which are open.\n\nabsent:\n  - what: OAuth 2.0 authorization server for public API access\n    status: not_found\n    note: No public OAuth client registration or authorization endpoint found.\n  - what: API key issuance for public read\n    status: not_applicable\n    note: All public surfaces read without credentials.\n  - what: Documented scope vocabulary\n    status: not_found\n    note: >-\n      No published scope list for any Caltech surface. This is why there is no scopes/\n      artifact in this repo — the absence is the finding.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caltech/refs/heads/main/authentication/caltech-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Private Research University
- Institute of Technology
- United States
- California
- Research Data
- Open Data
- Research Repository
- Identity Federation
- Astronomy
- Seismology
- Research Computing
- OAI-PMH
---
