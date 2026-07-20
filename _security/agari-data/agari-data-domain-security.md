---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: agari.com
  spf: true
hosts:
- cert_expires: Aug 25 17:24:55 2026 GMT
  host: www.agari.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 15:28:30 2026 GMT
  host: developers.agari.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 23:59:59 2026 GMT
  host: api.agari.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agari Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agari Data, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Agari Data
provider_slug: agari-data
slug: agari-data-domain-security
source_filename: agari-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.agari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:24:55 2026 GMT\n  hsts: null\n- host: developers.agari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 15:28:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.agari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: agari.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agari-data/refs/heads/main/security/agari-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email Security
- Phishing Protection
- DMARC
- Business Email Compromise
- Threat Intelligence
- Cybersecurity
---
