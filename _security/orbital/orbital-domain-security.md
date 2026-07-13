---
api_specs:
- filename: orbital-query-api-openapi.yml
  format: yaml
  label: Orbital Query API
  slug: query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/openapi/orbital-query-api-openapi.yml
- filename: orbital-schema-management-api-openapi.yml
  format: yaml
  label: Orbital Schema Management API
  slug: schema-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/openapi/orbital-schema-management-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: orbitalhq.com
  spf: false
hosts:
- cert_expires: Sep 30 02:53:48 2026 GMT
  host: orbitalhq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Orbital Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Orbital, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Orbital
provider_slug: orbital
slug: orbital-domain-security
source_filename: orbital-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: orbitalhq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 02:53:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: orbitalhq.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbital/refs/heads/main/security/orbital-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Data
- Gateways
---
