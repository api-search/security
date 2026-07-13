---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: carvana.com
  spf: true
hosts:
- cert_expires: Oct  6 06:59:36 2026 GMT
  host: www.carvana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 23:59:59 2026 GMT
  host: api-developer.carvana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 24 00:06:43 2026 GMT
  host: api.collective.carvana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Carvana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Carvana, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Carvana
provider_slug: carvana
slug: carvana-domain-security
source_filename: carvana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.carvana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 06:59:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-developer.carvana.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 10 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.collective.carvana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 00:06:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: carvana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/carvana/refs/heads/main/security/carvana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- E-Commerce
- Used Cars
- Inventory
- Partner API
- Fortune 500
---
