---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fm.com
  spf: true
hosts:
- cert_expires: Sep  7 21:16:44 2026 GMT
  host: www.fm.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Fm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FM (FM Global), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: FM (FM Global)
provider_slug: fm
slug: fm-domain-security
source_filename: fm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fm.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  7 21:16:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: fm.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fm/refs/heads/main/security/fm-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commercial Insurance
- Fortune 500
- Insurance
- Loss Prevention
- Property Insurance
- Risk Management
---
