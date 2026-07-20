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
  host: agari.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Agari Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Agari, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Agari
provider_slug: agari
slug: agari-domain-security
source_filename: agari-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agari.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 17:24:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: agari.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agari/refs/heads/main/security/agari-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Email Security
- Cybersecurity
- DMARC
- Email Authentication
- Phishing
- Anti-Phishing
- Brand Protection
- API
- REST
---
