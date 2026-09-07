---
api_specs:
- filename: acall-public-api-openapi.yml
  format: yaml
  label: Acall Public API
  slug: acall-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acall/refs/heads/main/openapi/acall-public-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: acall.inc
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: workstyleos.com
  spf: false
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: www.acall.inc
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.workstyleos.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: api.workstyleos.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Acall Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acall, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Acall
provider_slug: acall
slug: acall-domain-security
source_filename: acall-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acall.inc\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\n- host: www.workstyleos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\n- host: api.workstyleos.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: acall.inc\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: workstyleos.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acall/refs/heads/main/security/acall-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Workplace Management
- Visitor Management
- Meeting Room Booking
- Desk Booking
- Hybrid Work
- Access Control
- Facilities
- Smart Office
- Japan
- SaaS
---
