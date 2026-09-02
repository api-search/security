---
api_key_in: []
api_specs:
- filename: nura-bio-directory-api-openapi.yml
  format: yaml
  label: Nura Bio Directory API
  slug: nura-bio-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-directory-api-openapi.yml
- filename: nura-bio-discovery-api-openapi.yml
  format: yaml
  label: Nura Bio Discovery API
  slug: nura-bio-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-discovery-api-openapi.yml
- filename: nura-bio-media-api-openapi.yml
  format: yaml
  label: Nura Bio Media API
  slug: nura-bio-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-media-api-openapi.yml
- filename: nura-bio-pages-api-openapi.yml
  format: yaml
  label: Nura Bio Pages API
  slug: nura-bio-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-pages-api-openapi.yml
- filename: nura-bio-portfolio-api-openapi.yml
  format: yaml
  label: Nura Bio Portfolio API
  slug: nura-bio-portfolio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-portfolio-api-openapi.yml
- filename: nura-bio-posts-api-openapi.yml
  format: yaml
  label: Nura Bio Posts API
  slug: nura-bio-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-posts-api-openapi.yml
- filename: nura-bio-taxonomy-api-openapi.yml
  format: yaml
  label: Nura Bio Taxonomy API
  slug: nura-bio-taxonomy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/openapi/nura-bio-taxonomy-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Nura Bio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nura Bio declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Nura Bio
provider_slug: nura-bio
scheme_count: 2
schemes:
- applies_to: All 24 GET operations in openapi/nura-bio-content-api-openapi.yml. Verified anonymously on 2026-08-26.
  detail: No API key, token, cookie or signature is required or accepted for the catalogued read operations. The OpenAPI therefore declares no securitySchemes — an accurate absence, not an omission. Running 0-working/derive-authentication.py against this repo correctly returns zero schemes.
  id: none
  type: none
- advertised_at: https://nurabio.com/wp-json/
  applies_to: The authentication-gated remainder of the deployment. NOT part of the catalogued surface.
  authorization_endpoint: https://nurabio.com/wp-admin/authorize-application.php
  detail: The route index `authentication` object advertises WordPress Application Passwords and nothing else. These are per-user credentials minted from inside wp-admin by an existing site user; there is no registration, no developer signup and no public issuance path, so this is an administrative credential rather than an API product credential. Not exercised — API Evangelist holds no credentials for this site and never attempts to obtain any.
  id: application-passwords
  scheme: basic
  type: http
slug: nura-bio-authentication
source_filename: nura-bio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://nurabio.com/wp-json/ authentication block, plus live anonymous and gated responses observed\n  2026-08-26 against openapi/nura-bio-content-api-openapi.yml\nnote: >-\n  Nura Bio publishes no authentication documentation, because it publishes no developer program. This\n  profile is what the deployment actually does, read from the WordPress REST route index and confirmed\n  against live responses. The catalogued read surface requires NO credentials; the credentialed surface\n  exists but is for site administrators, not for API consumers, and no self-service path to a credential\n  is offered to the public.\nsummary:\n  anonymous_read: true\n  credential_required_for_catalogued_operations: false\n  self_service_credential_available: false\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\nschemes:\n- id: none\n  type: none\n  applies_to: >-\n    All 24 GET operations in openapi/nura-bio-content-api-openapi.yml.\
  \ Verified anonymously on 2026-08-26.\n  detail: >-\n    No API key, token, cookie or signature is required or accepted for the catalogued read operations. The\n    OpenAPI therefore declares no securitySchemes — an accurate absence, not an omission. Running\n    0-working/derive-authentication.py against this repo correctly returns zero schemes.\n- id: application-passwords\n  type: http\n  scheme: basic\n  applies_to: The authentication-gated remainder of the deployment. NOT part of the catalogued surface.\n  advertised_at: https://nurabio.com/wp-json/\n  authorization_endpoint: https://nurabio.com/wp-admin/authorize-application.php\n  detail: >-\n    The route index `authentication` object advertises WordPress Application Passwords and nothing else.\n    These are per-user credentials minted from inside wp-admin by an existing site user; there is no\n    registration, no developer signup and no public issuance path, so this is an administrative credential\n    rather than an API product\
  \ credential. Not exercised — API Evangelist holds no credentials for this\n    site and never attempts to obtain any.\ngated_surface_observed:\n  note: Observed anonymously on 2026-08-26; each returned the WordPress rest_forbidden envelope.\n  responses:\n  - path: /wp-json/wp/v2/settings\n    status: 401\n    code: rest_forbidden\n  - path: /wp-json/wp-abilities/v1/abilities\n    status: 401\n    code: rest_forbidden\n    detail: >-\n      The WordPress Abilities API registry — the layer a WordPress MCP adapter would expose as tools. Present\n      as a namespace but not anonymously enumerable, so no tool list could be read. See mcp/nura-bio-mcp.yml.\n  - path: /wp-json/aioseo/v1/options\n    status: 401\n    code: rest_forbidden\n  - path: /wp-json/aioseo/v1/ai-agents/mcp-adapter/release\n    status: 401\n    code: rest_forbidden\n  - path: /wp-json/wp/v2/comments\n    status: 403\n    code: rest_comment_disabled\n    detail: Comments are switched off site-wide, so the collection is\
  \ unreachable rather than credential-gated.\ncontext_parameter:\n  param: context\n  anonymous_values: [view, embed]\n  gated_values: [edit]\n  detail: >-\n    `context=edit` returns 401 rest_forbidden on every collection. The anonymous projection omits author\n    email, user roles, and unpublished content.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nura-bio/refs/heads/main/authentication/nura-bio-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Biotechnology
- Pharmaceuticals
- Neuroscience
- Neurodegeneration
- Drug Discovery
- Life Sciences
- Clinical Trials
- Rare Disease
- Small Molecule Therapeutics
- content-api
---
