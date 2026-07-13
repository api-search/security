---
api_specs:
- filename: warrant-dev-openapi.yml
  format: yaml
  label: Warrant Objects API
  slug: warrant-dev-objects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warrant-dev/refs/heads/main/openapi/warrant-dev-openapi.yml
- filename: warrant-dev-openapi.yml
  format: yaml
  label: Warrant Relationships (Warrants) API
  slug: warrant-dev-warrants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warrant-dev/refs/heads/main/openapi/warrant-dev-openapi.yml
- filename: warrant-dev-openapi.yml
  format: yaml
  label: Warrant Check (Authorization) API
  slug: warrant-dev-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warrant-dev/refs/heads/main/openapi/warrant-dev-openapi.yml
- filename: warrant-dev-openapi.yml
  format: yaml
  label: Warrant Object Types API
  slug: warrant-dev-object-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warrant-dev/refs/heads/main/openapi/warrant-dev-openapi.yml
- filename: warrant-dev-openapi.yml
  format: yaml
  label: Warrant Roles & Permissions API
  slug: warrant-dev-roles-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warrant-dev/refs/heads/main/openapi/warrant-dev-openapi.yml
description: ''
domains:
- caa: []
  dmarc: unknown
  dnssec: unknown
  domain: warrant.dev
  note: Not reconciled; hosted service retired.
  spf: unknown
hosts:
- host: warrant.dev
  https: true
  note: Marketing site remains and notes "Warrant -> Now WorkOS FGA".
- host: api.warrant.dev
  https: true
  note: RETIRED - hosted API sunset 2025-11-15; not probed.
- host: docs.warrant.dev
  https: false
  note: No longer resolves (DNS ENOTFOUND at review time); docs moved to workos.com/docs/fga.
kind: domain-security
layout: security
method: modeled
name: Warrant Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Warrant, probed live across 3 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS; 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present.'
provider_name: Warrant
provider_slug: warrant-dev
slug: warrant-dev-domain-security
source_filename: warrant-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: modeled\nsource: >-\n  Historical review of api.warrant.dev / warrant.dev. The standalone hosted\n  Warrant service was sunset 2025-11-15; live DNS/TLS/HTTP probes were not\n  performed because the hosted API host is retired and docs.warrant.dev no\n  longer resolves. Values below are not reconciled against live probes.\nhosts:\n- host: warrant.dev\n  https: true\n  note: Marketing site remains and notes \"Warrant -> Now WorkOS FGA\".\n- host: api.warrant.dev\n  https: true\n  note: RETIRED - hosted API sunset 2025-11-15; not probed.\n- host: docs.warrant.dev\n  https: false\n  note: No longer resolves (DNS ENOTFOUND at review time); docs moved to workos.com/docs/fga.\ndomains:\n- domain: warrant.dev\n  dnssec: unknown\n  caa: []\n  spf: unknown\n  dmarc: unknown\n  note: Not reconciled; hosted service retired.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warrant-dev/refs/heads/main/security/warrant-dev-domain-security.yml
summary_line: DNSSEC · DMARC
tags:
- Access Control
- Authorization
- Fine-Grained Authorization
- FGA
- RBAC
- ReBAC
- ABAC
- Zanzibar
- Permissions
- Open Source
- Retired
---
