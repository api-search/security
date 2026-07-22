---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wishup.co
  spf: true
hosts:
- cert_expires: Oct  3 09:53:39 2026 GMT
  host: wishup.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wishup Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wishup, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wishup
provider_slug: wishup
slug: wishup-domain-security
source_filename: wishup-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: wishup.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 09:53:39 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: wishup.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wishup/refs/heads/main/security/wishup-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Virtual Assistants
- Outsourcing
- Remote Work
- Bookkeeping
- Automation
- Staffing
- Productivity
---
