---
api_key_in: []
api_specs:
- filename: university-of-pennsylvania-accounts-user-api-openapi.yml
  format: yaml
  label: Penn Courses API (Penn Course Alert / Plan / Review / Degree Plan)
  slug: penn-courses
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-pennsylvania/refs/heads/main/openapi/university-of-pennsylvania-accounts-user-api-openapi.yml
- filename: university-of-pennsylvania-catalog-api-openapi.yml
  format: yaml
  label: University of Pennsylvania Catalog API
  slug: university-of-pennsylvania-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-pennsylvania/refs/heads/main/openapi/university-of-pennsylvania-catalog-api-openapi.yml
- filename: university-of-pennsylvania-request-api-openapi.yml
  format: yaml
  label: University of Pennsylvania Request API
  slug: university-of-pennsylvania-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-pennsylvania/refs/heads/main/openapi/university-of-pennsylvania-request-api-openapi.yml
auth_types: []
description: How each machine-readable surface attributed to the University of Pennsylvania authenticates, split by operator. Institution-operated surfaces are open-read library infrastructure plus a SAML identity provider; the course-registration surfaces that look like Penn APIs are operated by Penn Labs, a student organization, and authenticate against Penn Labs Accounts.
kind: authentication
layout: security
method: probed
name: University Of Pennsylvania Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Pennsylvania declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: University of Pennsylvania
provider_slug: university-of-pennsylvania
scheme_count: 0
schemes: []
slug: university-of-pennsylvania-authentication
source_filename: university-of-pennsylvania-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: University of Pennsylvania — Authentication Posture\naid: university-of-pennsylvania\ndescription: >-\n  How each machine-readable surface attributed to the University of Pennsylvania authenticates,\n  split by operator. Institution-operated surfaces are open-read library infrastructure plus a\n  SAML identity provider; the course-registration surfaces that look like Penn APIs are operated\n  by Penn Labs, a student organization, and authenticate against Penn Labs Accounts.\ngenerated: '2026-08-19'\nmethod: probed\nsource: live HTTP probes run 2026-08-19\nsurfaces:\n  - name: ScholarlyCommons at Penn — OAI-PMH\n    x-operator: institution\n    scheme: none\n    detail: >-\n      Anonymous harvesting. verb=Identify, ListSets, ListMetadataFormats and ListRecords all\n      returned 200 with no credential.\n    evidence:\n      - url: https://repository.upenn.edu/server/oai/request?verb=Identify\n        status: 200\n  - name: ScholarlyCommons at Penn — DSpace REST API\n\
  \    x-operator: institution\n    scheme: session\n    detail: >-\n      DSpace 7.6 REST. The API root and /server/api/authn are anonymous; content endpoints\n      require authentication. /server/api/core/items returned 401 with\n      {\"status\":401,\"error\":\"Unauthorized\",\"message\":\"Authentication is required\"}. Login,\n      logout and status links are advertised at /server/api/authn. Note the AUTHN CONTRACT IS\n      DSPACE'S, not Penn's engineering — Penn operates the deployment on its own domain.\n    evidence:\n      - url: https://repository.upenn.edu/server/api/authn\n        status: 200\n      - url: https://repository.upenn.edu/server/api/core/items?size=1\n        status: 401\n  - name: Penn Libraries Franklin catalog JSON\n    x-operator: institution\n    scheme: none\n    detail: >-\n      Anonymous read. /catalog.json and /catalog/{id}.json both returned 200 with no\n      credential, consistent with Penn Libraries' published open-metadata policy.\n    evidence:\n\
  \      - url: https://find.library.upenn.edu/catalog.json?q=penn\n        status: 200\n      - url: https://www.library.upenn.edu/about/policies/open-metadata\n        status: 200\n  - name: Colenda digital repository search JSON\n    x-operator: institution\n    scheme: none\n    detail: Anonymous read; Blacklight/Solr JSON returned 200 without credential.\n    evidence:\n      - url: https://colenda.library.upenn.edu/catalog.json?q=test\n        status: 200\n  - name: PennKey Identity Provider\n    x-operator: institution\n    scheme: saml\n    detail: >-\n      SAML 2.0 / Shibboleth identity provider. This is the surface Penn actually operates in\n      the authentication domain: a signed EntityDescriptor published at a well-known location\n      and resolvable through InCommon MDQ. It authenticates humans into relying parties, it is\n      not an API credential mechanism.\n    evidence:\n      - url: https://idp.pennkey.upenn.edu/idp/shibboleth\n        status: 200\n      - url: https://mdq.incommon.org/entities/https%3A%2F%2Fidp.pennkey.upenn.edu%2Fidp%2Fshibboleth\n\
  \        status: 200\n  - name: Penn Courses API (Penn Course Alert / Plan / Review / Degree Plan)\n    x-operator: tenant\n    x-operator-entity: Penn Labs\n    scheme: session\n    detail: >-\n      Mixed. Public course data reads anonymously — /api/base/current/search/courses/ returned\n      200 JSON. Anything user-scoped requires a Penn Labs Accounts session brokered by PennKey;\n      /api/review/course/CIS-120 returned 403 with\n      {\"detail\":\"Authentication credentials were not provided.\"}. The live OpenAPI at\n      /api/openapi/ declares NO components.securitySchemes, so the authentication requirement\n      is documented in prose only and is not machine-readable.\n    evidence:\n      - url: https://penncourseplan.com/api/base/current/search/courses/?search=CIS\n        status: 200\n      - url: https://penncoursereview.com/api/review/course/CIS-120\n        status: 403\n      - url: https://penncourseplan.com/api/openapi/\n        status: 200\n  - name: Penn Clubs API\n\
  \    x-operator: tenant\n    x-operator-entity: Penn Labs\n    scheme: session\n    detail: >-\n      Public club directory reads anonymously (/api/clubs returned 200 JSON); write and\n      membership operations require a Penn Labs Accounts session.\n    evidence:\n      - url: https://pennclubs.com/api/clubs?page=1\n        status: 200\ngaps:\n  - >-\n    No institution-operated surface publishes an OAuth 2.0 or OpenID Connect discovery\n    document. https://www.upenn.edu/.well-known/security.txt returned 404.\n  - >-\n    The one contract in this profile with a formal OpenAPI (Penn Courses) declares no security\n    schemes at all, despite enforcing authentication at runtime.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-pennsylvania/refs/heads/main/authentication/university-of-pennsylvania-authentication.yml
summary_line: 0 schemes
tags:
- Education
- Higher Education
- University
- Research University
- Ivy League
- United States
- Philadelphia
- Open Data
- Library
- Course Catalog
- Research Repository
- Identity Federation
- OAI-PMH
- Student Developers
---
