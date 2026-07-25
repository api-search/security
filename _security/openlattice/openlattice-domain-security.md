---
api_specs:
- filename: openlattice-authorizations-api-openapi.yml
  format: yaml
  label: OpenLattice authorizations API
  slug: openlattice-authorizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-authorizations-api-openapi.yml
- filename: openlattice-data-api-openapi.yml
  format: yaml
  label: OpenLattice data API
  slug: openlattice-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-data-api-openapi.yml
- filename: openlattice-edm-api-openapi.yml
  format: yaml
  label: OpenLattice edm API
  slug: openlattice-edm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-edm-api-openapi.yml
- filename: openlattice-organizations-api-openapi.yml
  format: yaml
  label: OpenLattice organizations API
  slug: openlattice-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-organizations-api-openapi.yml
- filename: openlattice-permissions-api-openapi.yml
  format: yaml
  label: OpenLattice permissions API
  slug: openlattice-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-permissions-api-openapi.yml
- filename: openlattice-principal-api-openapi.yml
  format: yaml
  label: OpenLattice principal API
  slug: openlattice-principal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-principal-api-openapi.yml
- filename: openlattice-search-api-openapi.yml
  format: yaml
  label: OpenLattice search API
  slug: openlattice-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-search-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: openlattice.com
  spf: true
hosts:
- host: openlattice.com
  https: false
- host: api.openlattice.com
  https: false
- host: api.staging.openlattice.com
  https: false
kind: domain-security
layout: security
method: probed
name: Openlattice Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenLattice, probed live across 3 host(s) and 1 registrable domain(s). Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenLattice
provider_slug: openlattice
slug: openlattice-domain-security
source_filename: openlattice-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openlattice.com\n  https: false\n- host: api.openlattice.com\n  https: false\n- host: api.staging.openlattice.com\n  https: false\ndomains:\n- domain: openlattice.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/security/openlattice-domain-security.yml
summary_line: no transport/DNS hardening detected
tags:
- Company
- Data Integration
- Entity Data Model
- Public Sector
- Analytics
- Graph
- Criminal Justice
---
