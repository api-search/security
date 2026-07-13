---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: triple-s-management.com
  spf: false
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: grupotriples.com
  spf: true
hosts:
- host: www.triple-s-management.com
  https: false
- cert_expires: Oct  5 21:35:19 2026 GMT
  host: management.grupotriples.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 23:59:59 2026 GMT
  host: service.ssspr.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Triple S Management Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Triple-S Management, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Triple-S Management
provider_slug: triple-s-management
slug: triple-s-management-domain-security
source_filename: triple-s-management-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.triple-s-management.com\n  https: false\n- host: management.grupotriples.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:35:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: service.ssspr.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 26 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: triple-s-management.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n- domain: grupotriples.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triple-s-management/refs/heads/main/security/triple-s-management-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Health Insurance
- Managed Care
- Medicare Advantage
- Puerto Rico
- Blue Cross Blue Shield
- Healthcare
---
