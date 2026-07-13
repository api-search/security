---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: amerco.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: uhaul.com
  spf: true
hosts:
- cert_expires: Oct  7 21:15:38 2026 GMT
  host: www.amerco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 12 23:59:59 2026 GMT
  host: www.uhaul.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Amerco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMERCO, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: AMERCO
provider_slug: amerco
slug: amerco-domain-security
source_filename: amerco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amerco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 21:15:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.uhaul.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 12 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: amerco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: uhaul.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amerco/refs/heads/main/security/amerco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Moving
- Storage
- Truck Rental
- Logistics
- Consumer Services
- Fortune 1000
---
