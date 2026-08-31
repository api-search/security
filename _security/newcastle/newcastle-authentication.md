---
api_key_in: []
api_specs:
- filename: newcastle-digitised-objects-api-openapi.yml
  format: yaml
  label: Digitised Objects Repository Search and Data API
  slug: digitised-objects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-digitised-objects-api-openapi.yml
- filename: newcastle-entity-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Entity
  slug: urban-observatory-entity
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-entity-api-openapi.yml
- filename: newcastle-feed-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Feed
  slug: urban-observatory-feed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-feed-api-openapi.yml
- filename: newcastle-summary-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Summary
  slug: urban-observatory-summary
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-summary-api-openapi.yml
- filename: newcastle-timeseries-api-openapi.yml
  format: yaml
  label: Urban Observatory API (Urban Sciences Building) — Timeseries
  slug: urban-observatory-timeseries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/openapi/newcastle-timeseries-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Newcastle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Newcastle University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Newcastle University
provider_slug: newcastle
scheme_count: 0
schemes: []
slug: newcastle-authentication
source_filename: newcastle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Newcastle University — authentication posture\naid: newcastle\ngenerated: '2026-08-30'\nmethod: derived\nx-evidence-method: probed\nsource: live probes of Newcastle University operated hosts, 2026-08-30\nsummary: >-\n  Every Newcastle University operated public API found in this profile is open and unauthenticated.\n  The institution's real authentication engineering is not in front of its APIs — it is its\n  federated SAML estate, which is machine-readable and institution-operated but is a login system,\n  not a programmable API.\napis:\n- aid: newcastle:digitised-objects\n  x-operator: institution\n  scheme: none\n  detail: >-\n    The OpenAPI at https://api-dor.ncl.ac.uk/info/open-api declares no securitySchemes and no\n    top-level security requirement. GET https://api-dor.ncl.ac.uk/v1/collections returns 200 with\n    data and no credential.\n  verified: '2026-08-30'\n- aid: newcastle:ecppec\n  x-operator: institution\n  scheme: none\n  detail: >-\n    The GraphQL\
  \ endpoint accepts unauthenticated POST queries and leaves introspection open.\n    Verified 2026-08-30 with an anonymous query returning real constituency records.\n  verified: '2026-08-30'\n- aid: newcastle:urban-observatory\n  x-operator: institution\n  scheme: none\n  detail: >-\n    No securitySchemes in the Urban Sciences Building OpenAPI. GET\n    /api/v2.0a/sensors/entity returned 200 and 616 entities anonymously on 2026-08-30. Some\n    operations note that results are returned \"provided permissions permit\", which is a\n    server-side data visibility rule rather than a caller credential.\n  verified: '2026-08-30'\n- aid: newcastle:etheses-oai\n  x-operator: institution\n  scheme: none\n  detail: OAI-PMH is an open harvesting protocol; verb=Identify returns 200 with no credential.\n  verified: '2026-08-30'\n- aid: newcastle:data-ncl\n  x-operator: tenant\n  scheme: vendor\n  detail: >-\n    data.ncl.ac.uk is a Figshare tenant (CNAME to figshare.com). Programmatic access runs\
  \ on\n    Figshare's OAuth 2.0 and personal-token scheme, documented and operated by Figshare, not by\n    Newcastle. Not scored here.\nidentity_federation:\n  x-operator: institution\n  protocol: SAML 2.0 / Shibboleth\n  entity_id: https://gateway.ncl.ac.uk/idp/shibboleth\n  metadata_url: https://gateway.ncl.ac.uk/idp/shibboleth\n  scope: ncl.ac.uk\n  federation: UK Access Management Federation (feeds eduGAIN)\n  federation_metadata: http://metadata.ukfederation.org.uk/ukfederation-metadata.xml\n  sso_endpoints:\n  - https://gateway.ncl.ac.uk/idp/profile/SAML2/Redirect/SSO\n  - https://gateway.ncl.ac.uk/idp/profile/SAML2/POST/SSO\n  - https://gateway.ncl.ac.uk/idp/profile/SAML2/POST-SimpleSign/SSO\n  - https://gateway.ncl.ac.uk/idp/profile/Shibboleth/SSO\n  service_providers_registered: 168\n  development_idp: https://dev-gateway.ncl.ac.uk/idp/shibboleth\n  verified: '2026-08-30'\n  detail: >-\n    This is the largest genuinely institution-operated machine-readable surface Newcastle has.\
  \ It is\n    a login federation, not a data API, and it is recorded here rather than as an apis[] contract\n    with request/response semantics.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newcastle/refs/heads/main/authentication/newcastle-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- United Kingdom
- Russell Group
- Research Data
- Open Data
- Digital Library
- Identity Federation
- Smart Cities
- Cultural Heritage
---
