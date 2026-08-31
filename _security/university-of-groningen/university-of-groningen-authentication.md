---
api_key_in: []
api_specs:
- filename: university-of-groningen-course-catalog-api-openapi.yml
  format: yaml
  label: University of Groningen Ocasys Course Catalog API
  slug: ocasys-course-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-groningen/refs/heads/main/openapi/university-of-groningen-course-catalog-api-openapi.yml
- filename: university-of-groningen-oai-pmh-openapi.yml
  format: yaml
  label: University of Groningen Research Database OAI-PMH
  slug: pure-oai-pmh
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-groningen/refs/heads/main/openapi/university-of-groningen-oai-pmh-openapi.yml
auth_types: []
description: 'How access actually works across the University of Groningen''s programmable surfaces, established by calling each one on 2026-08-30. There is no institutional developer portal, no API key issuance and no self-service registration anywhere in this footprint. Access is one of three things: fully open, gated behind the University''s SAML single sign-on, or gated behind a key that a vendor''s platform issues to the institution rather than to a developer.'
kind: authentication
layout: security
method: probed
name: University Of Groningen Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Groningen declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: University of Groningen
provider_slug: university-of-groningen
scheme_count: 4
schemes:
- description: Course search, course detail, programme search, faculties, option lists and academic years answer 200 to an unauthenticated GET with no key, no token and no Origin restriction observed.
  evidence:
    status: 200
    url: https://ocasys.rug.nl/api/2026-2027/course?searchTerm=biology
  name: none
  operator: institution
  surface: Ocasys course catalog API (ocasys.rug.nl/api) — read paths
  type: open
- description: All OAI-PMH verbs answer unauthenticated; harvesting is open, subject to polite use.
  evidence:
    status: 200
    url: https://pure.rug.nl/ws/oai?verb=Identify
  name: none
  operator: institution
  surface: UG Research Portal OAI-PMH (pure.rug.nl/ws/oai)
  type: open
- description: 'Institutional single sign-on via the University''s own SAML 2.0 identity provider at signon.rug.nl, federated through SURFconext and eduGAIN. There is no public route to a session: an account is issued to affiliates, not to developers. The gated Ocasys endpoints return a bare 403 with no problem body and no WWW-Authenticate hint.'
  evidence:
    status: 403
    url: https://ocasys.rug.nl/api/2026-2027/course-offering?permission=READ
  name: saml-sso
  operator: institution
  surface: Gated Ocasys paths, the Rooster timetable app, and staff/student systems
  type: federated
- description: The Pure web-services API requires an api-key header. The key is provisioned by the University to its own integrations through the Pure administration console; there is no public request form. The contract, the documentation and the scheme are Elsevier's — pure.rug.nl/ws/api redirects to a documentation page whose canonical link is api.elsevierpure.com — so this is recorded as a tenant deployment rather than a University of Groningen API.
  evidence:
    note: Redirects to /ws/api/documentation/index.html with rel=canonical https://api.elsevierpure.com/ws/api/documentation/index.html
    status: 200
    url: https://pure.rug.nl/ws/api
  in: header
  name: api-key
  operator: tenant
  parameter: api-key
  surface: Elsevier Pure REST API deployed at pure.rug.nl/ws/api
  type: apiKey
slug: university-of-groningen-authentication
source_filename: university-of-groningen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\nprovider: University of Groningen\nproviderId: university-of-groningen\ngenerated: '2026-08-30'\nmethod: probed\nx-operator: institution\ndescription: >-\n  How access actually works across the University of Groningen's programmable surfaces, established\n  by calling each one on 2026-08-30. There is no institutional developer portal, no API key issuance\n  and no self-service registration anywhere in this footprint. Access is one of three things: fully\n  open, gated behind the University's SAML single sign-on, or gated behind a key that a vendor's\n  platform issues to the institution rather than to a developer.\nsource:\n  - https://ocasys.rug.nl/api/2026-2027/course?searchTerm=biology\n  - https://ocasys.rug.nl/api/2026-2027/course-offering?permission=READ\n  - https://pure.rug.nl/ws/oai?verb=Identify\n  - https://pure.rug.nl/ws/api\n  - https://signon.rug.nl/nidp/saml2/metadata\nschemes:\n  - name:\
  \ none\n    type: open\n    surface: Ocasys course catalog API (ocasys.rug.nl/api) — read paths\n    operator: institution\n    description: >-\n      Course search, course detail, programme search, faculties, option lists and academic years\n      answer 200 to an unauthenticated GET with no key, no token and no Origin restriction observed.\n    evidence:\n      url: https://ocasys.rug.nl/api/2026-2027/course?searchTerm=biology\n      status: 200\n  - name: none\n    type: open\n    surface: UG Research Portal OAI-PMH (pure.rug.nl/ws/oai)\n    operator: institution\n    description: All OAI-PMH verbs answer unauthenticated; harvesting is open, subject to polite use.\n    evidence:\n      url: https://pure.rug.nl/ws/oai?verb=Identify\n      status: 200\n  - name: saml-sso\n    type: federated\n    surface: Gated Ocasys paths, the Rooster timetable app, and staff/student systems\n    operator: institution\n    description: >-\n      Institutional single sign-on via the University's own\
  \ SAML 2.0 identity provider at\n      signon.rug.nl, federated through SURFconext and eduGAIN. There is no public route to a session:\n      an account is issued to affiliates, not to developers. The gated Ocasys endpoints return a bare\n      403 with no problem body and no WWW-Authenticate hint.\n    evidence:\n      url: https://ocasys.rug.nl/api/2026-2027/course-offering?permission=READ\n      status: 403\n  - name: api-key\n    type: apiKey\n    in: header\n    parameter: api-key\n    surface: Elsevier Pure REST API deployed at pure.rug.nl/ws/api\n    operator: tenant\n    description: >-\n      The Pure web-services API requires an api-key header. The key is provisioned by the University\n      to its own integrations through the Pure administration console; there is no public request\n      form. The contract, the documentation and the scheme are Elsevier's — pure.rug.nl/ws/api\n      redirects to a documentation page whose canonical link is api.elsevierpure.com — so this is\n\
  \      recorded as a tenant deployment rather than a University of Groningen API.\n    evidence:\n      url: https://pure.rug.nl/ws/api\n      status: 200\n      note: Redirects to /ws/api/documentation/index.html with rel=canonical https://api.elsevierpure.com/ws/api/documentation/index.html\nnotes: >-\n  No OAuth 2.0, no OpenID Connect client registration and no personal access tokens were found on any\n  University of Groningen host. For an agent, the practical answer is that the course catalog and the\n  OAI-PMH endpoint are callable today and everything else is closed.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-groningen/refs/heads/main/authentication/university-of-groningen-authentication.yml
summary_line: 4 schemes
tags:
- Education
- Higher Education
- University
- Netherlands
- Europe
- Research
- Research Data
- Course Catalog
- Identity Federation
- OAI-PMH
- Library
- Metadata
- Open Data
---
