---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kymetacorp.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kymeta.io
  spf: true
hosts:
- cert_expires: Oct 13 07:55:43 2026 GMT
  host: www.kymetacorp.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 16:58:49 2026 GMT
  host: api.kymeta.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  hsts_note: 'probe-domain-security.py recorded hsts null for this host; a re-probe of both HEAD / and GET /health returned "strict-transport-security: max-age=31536000; includeSubDomains", so the corrected observed value is recorded here.'
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 16:58:49 2026 GMT
  host: access.kymeta.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kymeta Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kymeta, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kymeta
provider_slug: kymeta
slug: kymeta-domain-security
source_filename: kymeta-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.kymetacorp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 07:55:43 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: api.kymeta.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 16:58:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  hsts_note: >-\n    probe-domain-security.py recorded hsts null for this host; a re-probe of both HEAD /\n    and GET /health returned \"strict-transport-security: max-age=31536000; includeSubDomains\",\n    so the corrected observed value is recorded here.\n- host: access.kymeta.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 16:58:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kymetacorp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: kymeta.io\n  dnssec:\
  \ false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\nnotes:\n  - No CAA record on either kymetacorp.com or kymeta.io, so certificate issuance is not pinned to\n    a named CA.\n  - No DNSSEC on either registrable domain.\n  - DMARC is published on both domains at p=quarantine rather than p=reject.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kymeta/refs/heads/main/security/kymeta-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Satellite
- Satellite Communications
- Connectivity
- Telecommunications
- Networking
- Antennas
- Metamaterials
- Aerospace and Defense
- Maritime
- Remote Monitoring
- Hardware
---
