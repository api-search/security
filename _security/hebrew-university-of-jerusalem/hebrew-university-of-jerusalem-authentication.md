---
api_key_in: []
api_specs:
- filename: hebrew-university-of-jerusalem-shnaton-course-catalog-openapi.yml
  format: yaml
  label: Shnaton Course Catalog API
  slug: shnaton-course-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hebrew-university-of-jerusalem/refs/heads/main/openapi/hebrew-university-of-jerusalem-shnaton-course-catalog-openapi.yml
auth_types: []
description: 'Authentication across the Hebrew University of Jerusalem''s programmable surfaces. The headline is that the one institution-operated API found in this profile requires no authentication at all, and the university operates no API key issuance, no OAuth authorization server, and no developer registration of any kind that could be found. Human and staff authentication is a different story and is entirely SAML: a university-run SimpleSAMLphp identity provider at idp.cc.huji.ac.il fronts the institutional web estate, including the vendor platforms the university is a tenant of.'
kind: authentication
layout: security
method: probed
name: Hebrew University Of Jerusalem Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hebrew University of Jerusalem declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Hebrew University of Jerusalem
provider_slug: hebrew-university-of-jerusalem
scheme_count: 0
schemes: []
slug: hebrew-university-of-jerusalem-authentication
source_filename: hebrew-university-of-jerusalem-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "# x-method: derived\n# x-source-url: https://shnaton.huji.ac.il/api\n# Authored by API Evangelist from live probes of the Hebrew University of Jerusalem's own\n# hosts. NOT published by the institution. See `method:` below for how it was obtained.\nspecification: API Evangelist Authentication\nspecificationVersion: '0.1'\nprovider: Hebrew University of Jerusalem\nproviderId: hebrew-university-of-jerusalem\ngenerated: '2026-09-01'\nmethod: probed\nsource: >-\n  Live unauthenticated requests to https://shnaton.huji.ac.il/api on 2026-09-01 with no\n  credential of any kind, plus an authenticated-surface probe of\n  https://cris.huji.ac.il/admin/workspace.xhtml and a fetch of the SAML 2.0 metadata at\n  https://idp.cc.huji.ac.il/simplesaml/saml2/idp/metadata.php (HTTP 200, application/xml,\n  4,548 bytes).\ndescription: >-\n  Authentication across the Hebrew University of Jerusalem's programmable surfaces. The\n  headline is that the one institution-operated API found in this profile\
  \ requires no\n  authentication at all, and the university operates no API key issuance, no OAuth\n  authorization server, and no developer registration of any kind that could be found.\n  Human and staff authentication is a different story and is entirely SAML: a\n  university-run SimpleSAMLphp identity provider at idp.cc.huji.ac.il fronts the\n  institutional web estate, including the vendor platforms the university is a tenant of.\n\nsurfaces:\n  - name: Shnaton Course Catalog API\n    baseURL: https://shnaton.huji.ac.il/api\n    x-operator: institution\n    scheme: none\n    authenticated: false\n    registration_required: false\n    key_issuance: none\n    detail: >-\n      Every operation was called with no Authorization header, no cookie, no API key and no\n      referer, and every one returned its full production payload. There is no 401 path in\n      this API — the only error responses observed were 400 for a missing or malformed\n      parameter and 404 for an unrouted path.\
  \ A single unauthenticated POST to\n      /courses/search-advanced returned 14,153,560 bytes covering 6,355 courses, which\n      means the entire published course catalog is readable anonymously.\n    evidence:\n      - url: https://shnaton.huji.ac.il/api/faculties\n        status: 200\n        note: No credential sent; full response returned.\n      - url: https://shnaton.huji.ac.il/api/courses/search-advanced?include=1\n        status: 200\n        note: Unauthenticated POST, 14,153,560-byte response.\n    security_headers_observed:\n      - 'X-Content-Type-Options: nosniff'\n      - 'X-Frame-Options: DENY'\n      - 'Strict-Transport-Security: max-age=31536000; includeSubDomains'\n      - 'X-HujiShnatonServer: Server 2'\n\n  - name: Hebrew University SAML Identity Provider\n    entityID: https://idp.cc.huji.ac.il/simplesaml/saml2/idp/metadata.php\n    x-operator: institution\n    scheme: saml2\n    implementation: SimpleSAMLphp\n    authenticated: true\n    detail: >-\n      The university's\
  \ own SAML 2.0 identity provider, run by the Authority for Computation,\n      Communication and Information (cc.huji.ac.il). The signing certificate embedded in the\n      metadata carries subject O=Hebrew University, OU=The authority for computation,\n      communication and information, CN=idp1.cc.huji.ac.il, emailAddress=ssobox@cc.huji.ac.il\n      — the institution's own key, not a managed federation service's. This is the strongest\n      machine-readable authentication contract the university publishes.\n    evidence:\n      - url: https://idp.cc.huji.ac.il/simplesaml/saml2/idp/metadata.php\n        status: 200\n        note: SAML 2.0 EntityDescriptor with IDPSSODescriptor, application/xml.\n\n  - name: Elsevier Pure CRIS (cris.huji.ac.il)\n    x-operator: tenant\n    scheme: saml2\n    detail: >-\n      The research portal's administrative surface redirects unauthenticated callers to the\n      university's own IdP, which is how the tenant relationship was confirmed from the\n\
  \      authentication path rather than from the hostname alone. The Pure web services API at\n      /ws/api requires an Elsevier-issued API key the university holds and does not publish;\n      an unauthenticated request for its OpenAPI returned HTTP 401. The public OAI-PMH\n      endpoint at /ws/oai is unauthenticated.\n    evidence:\n      - url: https://cris.huji.ac.il/admin/workspace.xhtml\n        status: 200\n        note: Redirects to idp.cc.huji.ac.il SSOService with spentityid=https://cris.huji.ac.il/admin.\n      - url: https://cris.huji.ac.il/ws/api/524/openapi.yaml\n        status: 401\n        note: Pure API contract is key-gated; the key is Elsevier-issued and not public.\n      - url: https://cris.huji.ac.il/ws/oai?verb=Identify\n        status: 200\n        note: OAI-PMH is open, no credential required.\n\nabsent:\n  - what: API key issuance\n    detail: No developer registration, key request form or self-service portal was found on any huji.ac.il host.\n  - what: OAuth\
  \ 2.0 / OpenID Connect\n    detail: No authorization server, no .well-known/openid-configuration on any probed host.\n  - what: Developer portal\n    detail: api.huji.ac.il and developer.huji.ac.il do not resolve (NXDOMAIN).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hebrew-university-of-jerusalem/refs/heads/main/authentication/hebrew-university-of-jerusalem-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Research
- Israel
- Jerusalem
- Course Catalog
- Identity Federation
- Research Repository
- Library
- SAML
- OAI-PMH
- Open Access
- Public Research University
---
