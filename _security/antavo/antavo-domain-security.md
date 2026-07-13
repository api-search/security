---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: antavo.com
  spf: true
hosts:
- cert_expires: Aug 17 22:27:21 2026 GMT
  host: antavo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  6 04:03:04 2026 GMT
  host: developers.antavo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 21:13:31 2026 GMT
  host: api.antavo.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Antavo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Antavo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Antavo
provider_slug: antavo
slug: antavo-domain-security
source_filename: antavo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: antavo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 17 22:27:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.antavo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  6 04:03:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.antavo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 21:13:31 2026 GMT\n  hsts: null\ndomains:\n- domain: antavo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/antavo/refs/heads/main/security/antavo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Loyalty
- Customer Loyalty
- Rewards
- Enterprise
- Headless
- Retail
- Marketing
- Engagement
---
