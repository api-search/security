---
api_specs:
- filename: openlattice-openapi.yaml
  format: yaml
  label: OpenLattice API
  slug: openlattice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openlattice/refs/heads/main/openapi/openlattice-openapi.yaml
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
