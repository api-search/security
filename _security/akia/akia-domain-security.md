---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: akia.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: akia.ai
  spf: true
hosts:
- cert_expires: Oct 15 14:28:06 2026 GMT
  host: www.akia.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 15:23:57 2026 GMT
  host: api.akia.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 16:24:30 2026 GMT
  host: sys.akia.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akia Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akia, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Akia
provider_slug: akia
slug: akia-domain-security
source_filename: akia-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 14:28:06 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.akia.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 15:23:57 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: sys.akia.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 16:24:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: akia.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: akia.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akia/refs/heads/main/security/akia-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Hospitality
- Hotels
- Vacation Rentals
- Guest Experience
- Messaging
- Artificial Intelligence
- Agents
- Property Management
- Check-in
---
