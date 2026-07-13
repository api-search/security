---
api_specs:
- filename: openapi
  format: yaml
  label: Northbeam Orders API
  slug: orders-api
  spec_type: OpenAPI
  url: https://docs.northbeam.io/openapi
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: northbeam.io
  spf: true
hosts:
- cert_expires: Oct  1 02:03:36 2026 GMT
  host: www.northbeam.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  1 17:43:11 2026 GMT
  host: docs.northbeam.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 25 11:33:49 2026 GMT
  host: api.northbeam.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Northbeam Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Northbeam, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Northbeam
provider_slug: northbeam
slug: northbeam-domain-security
source_filename: northbeam-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.northbeam.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 02:03:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.northbeam.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 17:43:11 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.northbeam.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 25 11:33:49 2026 GMT\n  hsts: null\ndomains:\n- domain: northbeam.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/northbeam/refs/heads/main/security/northbeam-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Marketing Attribution
- Multi-Touch Attribution
- E-Commerce
- ROAS
- Media Mix Modeling
- Creative Analytics
- Performance Marketing
---
