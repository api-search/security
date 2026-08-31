---
api_key_in: []
api_specs:
- filename: stanford-about-api-openapi.yml
  format: yaml
  label: Stanford University About API
  slug: stanford-about-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-about-api-openapi.yml
- filename: stanford-authentication-api-openapi.yml
  format: yaml
  label: Stanford University Authentication API
  slug: stanford-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-authentication-api-openapi.yml
- filename: stanford-catalog-api-openapi.yml
  format: yaml
  label: Stanford University Catalog API
  slug: stanford-catalog-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-catalog-api-openapi.yml
- filename: stanford-events-api-openapi.yml
  format: yaml
  label: Stanford University Events API
  slug: stanford-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-events-api-openapi.yml
- filename: stanford-files-api-openapi.yml
  format: yaml
  label: Stanford University Files API
  slug: stanford-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-files-api-openapi.yml
- filename: stanford-identifiers-api-openapi.yml
  format: yaml
  label: Stanford University Identifiers API
  slug: stanford-identifiers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-identifiers-api-openapi.yml
- filename: stanford-integrations-api-openapi.yml
  format: yaml
  label: Stanford University Integrations API
  slug: stanford-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-integrations-api-openapi.yml
- filename: stanford-jobs-api-openapi.yml
  format: yaml
  label: Stanford University Jobs API
  slug: stanford-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-jobs-api-openapi.yml
- filename: stanford-legacy-api-openapi.yml
  format: yaml
  label: Stanford University Legacy API
  slug: stanford-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-legacy-api-openapi.yml
- filename: stanford-metadata-api-openapi.yml
  format: yaml
  label: Stanford University Metadata API
  slug: stanford-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-metadata-api-openapi.yml
- filename: stanford-objects-api-openapi.yml
  format: yaml
  label: Stanford University Objects API
  slug: stanford-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-objects-api-openapi.yml
- filename: stanford-release-tags-api-openapi.yml
  format: yaml
  label: Stanford University Release Tags API
  slug: stanford-release-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-release-tags-api-openapi.yml
- filename: stanford-tags-api-openapi.yml
  format: yaml
  label: Stanford University Tags API
  slug: stanford-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-tags-api-openapi.yml
- filename: stanford-versions-api-openapi.yml
  format: yaml
  label: Stanford University Versions API
  slug: stanford-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-versions-api-openapi.yml
- filename: stanford-workflows-api-openapi.yml
  format: yaml
  label: Stanford University Workflows API
  slug: stanford-workflows-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-workflows-api-openapi.yml
- filename: stanford-workspaces-api-openapi.yml
  format: yaml
  label: Stanford University Workspaces API
  slug: stanford-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/openapi/stanford-workspaces-api-openapi.yml
auth_types: []
description: 'How access is established across Stanford''s institution-operated API surfaces. Stanford runs four distinct authentication regimes rather than one developer-portal key: an open/anonymous tier for library discovery data, a bearer-token tier for the Stanford Digital Repository backends, an x509 client-certificate tier for the MaIS Registry, and campus SSO (Shibboleth SAML 2.0 / OIDC) for everything a human logs into. No public self-service key issuance exists for any of them; every credentialed surface is requested through a Stanford support workflow.'
kind: authentication
layout: security
method: derived
name: Stanford Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stanford University declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Stanford University
provider_slug: stanford
scheme_count: 0
schemes: []
slug: stanford-authentication
source_filename: stanford-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "name: Stanford University — authentication\ndescription: >-\n  How access is established across Stanford's institution-operated API surfaces. Stanford runs\n  four distinct authentication regimes rather than one developer-portal key: an open/anonymous\n  tier for library discovery data, a bearer-token tier for the Stanford Digital Repository\n  backends, an x509 client-certificate tier for the MaIS Registry, and campus SSO (Shibboleth\n  SAML 2.0 / OIDC) for everything a human logs into. No public self-service key issuance exists\n  for any of them; every credentialed surface is requested through a Stanford support workflow.\ngenerated: '2026-08-19'\nmodified: '2026-08-19'\nmethod: derived\nsource: >-\n  Derived from openapi/_original/*.yml (components.securitySchemes + security), from the live\n  Shibboleth metadata at https://idp.stanford.edu/metadata.xml, and from the credential language\n  on https://uit.stanford.edu/developers/apis and https://uit.stanford.edu/service/ai-api-gateway.\n\
  x-operator: institution\nmechanisms:\n  - id: anonymous-public\n    name: Open / no credential\n    type: none\n    method: probed\n    source: live 200 responses, 2026-08-19\n    applies_to:\n      - Stanford Libraries PURL API\n      - Stanford Libraries IIIF API\n      - Stanford Libraries Library Hours API\n      - ExploreCourses XML query interface\n    evidence:\n      - url: https://purl.stanford.edu/bb157hs6068.xml\n        status: 200\n      - url: https://library-hours.stanford.edu/libraries.json\n        status: 200\n      - url: https://purl.stanford.edu/bb157hs6068/iiif/manifest\n        status: 200\n      - url: https://explorecourses.stanford.edu/search?view=xml-20140630&q=CS106A&academicYear=20242025\n        status: 200\n    note: >-\n      These four answer to an anonymous client with no header of any kind. This is the widest\n      genuinely open API surface Stanford operates.\n  - id: bearer-token\n    name: HTTP bearer token\n    type: http\n    scheme: bearer\n  \
  \  method: derived\n    source: components.securitySchemes.bearerAuth in the SDR contracts\n    applies_to:\n      - SDR API\n      - DOR Services API\n      - Preservation Catalog HTTP API\n    declared_in:\n      - openapi/_original/stanford-sdr-api-openapi.yml\n      - openapi/_original/stanford-dor-services-api-openapi.yml\n      - openapi/_original/stanford-preservation-catalog-api-openapi.yml\n    issuance: >-\n      Not self-service and not publicly documented. The SDR API contract exposes POST /v1/auth/login,\n      but the services themselves sit on the Stanford internal network — sdr-api-prod.stanford.edu\n      resolves in public DNS and does not answer a public TCP connection.\n    note: >-\n      Contract-declared, deployment-gated. The security scheme is a fact about the published\n      contract, not a claim that a member of the public can obtain a token.\n  - id: no-declared-scheme\n    name: No security scheme declared\n    type: none\n    method: derived\n    source:\
  \ absence of a security block in the source contracts\n    applies_to:\n      - Technical Metadata API\n      - SURI API\n    note: >-\n      Neither contract declares security. Both are internal SDR backends whose hostnames do not\n      resolve in public DNS (technical-metadata-prod.stanford.edu, sul-suri-prod.stanford.edu are\n      NXDOMAIN), so the absence reflects network placement rather than an open surface. This is a\n      contract-quality gap worth reporting to sul-dlss, not an access route.\n  - id: x509-client-certificate\n    name: x509 client certificate (mutual TLS)\n    type: mutualTLS\n    method: searched\n    source: https://uit.stanford.edu/developers/apis\n    applies_to:\n      - MaIS Registry APIs (Account, Person, Student, CourseClass, Privilege, Workgroup)\n    issuance: >-\n      Certificate signed by the Stanford MaIS team, requested through the UIT developer\n      onboarding checklist. No sandbox, no public base URL, no anonymous tier.\n    evidence:\n   \
  \   - url: https://uit.stanford.edu/developers/apis\n        status: 200\n      - url: https://uit.stanford.edu/developers/apis/getting-started\n        status: 200\n  - id: api-key\n    name: Issued API key\n    type: apiKey\n    method: searched\n    source: https://uit.stanford.edu/service/ai-api-gateway\n    applies_to:\n      - Stanford AI API Gateway\n    issuance: >-\n      Requested through the ServiceNow catalog; requires a valid Stanford PTA (billing account).\n      Metered and rate-carded — usage is queryable by API key.\n    evidence:\n      - url: https://uit.stanford.edu/service/ai-api-gateway\n        status: 200\n  - id: shibboleth-sso\n    name: Campus SSO — Shibboleth SAML 2.0 and OIDC\n    type: federated\n    method: probed\n    source: https://idp.stanford.edu/metadata.xml\n    applies_to:\n      - CAP / Stanford Profiles API console\n      - AI Playground\n      - Stanford Community of Practice\n    entity_id: https://idp.stanford.edu/\n    protocols:\n      - urn:oasis:names:tc:SAML:2.0:protocol\n\
  \      - openid-connect\n    bindings:\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST-SimpleSign\n      - urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    sso_endpoint: https://login.stanford.edu/idp/profile/SAML2/POST/SSO\n    oidc_authorize: https://login.stanford.edu/idp/profile/oidc/authorize\n    evidence:\n      - url: https://idp.stanford.edu/metadata.xml\n        status: 200\n      - url: https://aiplayground.stanford.edu/\n        status: 200\n        note: redirects to login.stanford.edu/idp/profile/oidc/authorize\n      - url: https://cap.stanford.edu/cap-api/console\n        status: 303\n        note: redirects to authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stanford/refs/heads/main/authentication/stanford-authentication.yml
summary_line: 0 schemes
tags:
- University
- Higher Education
- Education
- Research
- United States
- California
- Private Research University
- Association of American Universities
- Research Repository
- Course Catalog
- Identity Federation
- Library
- Digital Repository
- Artificial Intelligence
- IIIF
---
