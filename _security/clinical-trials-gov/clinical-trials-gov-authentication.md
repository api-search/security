---
anonymous_access: false
api_key_in: []
api_specs:
- filename: clinical-trials-gov-stats-api-openapi.yml
  format: yaml
  label: ClinicalTrials.gov Stats API
  slug: clinical-trials-gov-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clinical-trials-gov/refs/heads/main/openapi/clinical-trials-gov-stats-api-openapi.yml
- filename: clinical-trials-gov-studies-api-openapi.yml
  format: yaml
  label: ClinicalTrials.gov Studies API
  slug: clinical-trials-gov-studies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clinical-trials-gov/refs/heads/main/openapi/clinical-trials-gov-studies-api-openapi.yml
- filename: clinical-trials-gov-version-api-openapi.yml
  format: yaml
  label: ClinicalTrials.gov Version API
  slug: clinical-trials-gov-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clinical-trials-gov/refs/heads/main/openapi/clinical-trials-gov-version-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Clinical Trials Gov Authentication
name_suffix: Authentication
oauth_flows: []
overview: ClinicalTrials.gov declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: ClinicalTrials.gov
provider_slug: clinical-trials-gov
scheme_count: 0
schemes: []
slug: clinical-trials-gov-authentication
source_filename: clinical-trials-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: >-\n  openapi/_original/clinical-trials-gov-openapi.yml (no securitySchemes) plus live\n  unauthenticated probes of https://clinicaltrials.gov/api/v2/* on 2026-09-06\nsummary:\n  authentication_required: false\n  scheme_count: 0\n  registration_required: false\n  api_key_required: false\n  oauth: false\nschemes: []\nfinding: >-\n  The ClinicalTrials.gov Data API v2 requires no authentication of any kind. No\n  securityScheme is declared in the contract, no credential is requested anywhere on\n  https://clinicaltrials.gov/data-api, and unauthenticated GETs against every documented\n  path return 200 with data. There is no signup, no key issuance and no account.\nevidence:\n- url: https://clinicaltrials.gov/api/v2/studies?pageSize=1\n  status: 200\n  note: unauthenticated, returned a full study record (application/json)\n- url: https://clinicaltrials.gov/api/v2/version\n  status: 200\n  note: unauthenticated\n- url: https://clinicaltrials.gov/api/v2/studies/metadata\n\
  \  status: 200\n  note: unauthenticated, 175,633 bytes of field metadata\n- url: https://clinicaltrials.gov/.well-known/oauth-authorization-server\n  status: 200\n  note: SPA HTML shell, not an authorization-server metadata document — no OAuth surface exists\ntransport:\n  https_required: true\n  tls_version: TLSv1.3\n  hsts: true\n  note: See security/clinical-trials-gov-domain-security.yml for the full TLS/DNS posture.\ndata_rights:\n  note: >-\n    Data is U.S. Government work in the public domain and available \"to all requesters, both\n    within and outside the United States, at no charge\"\n    (https://clinicaltrials.gov/about-site/terms-conditions). Some records may carry\n    third-party copyright; the terms tell consumers to consult those entities directly.\n    Attribution to NLM and ClinicalTrials.gov is requested.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clinical-trials-gov/refs/heads/main/authentication/clinical-trials-gov-authentication.yml
summary_line: 0 schemes
tags:
- Clinical Trials
- Government
- Health
- NIH
- Open Data
- Public Health
- Research
---
