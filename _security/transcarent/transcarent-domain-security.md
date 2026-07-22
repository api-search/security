---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: transcarent.ai
  spf: true
hosts:
- cert_expires: Oct  9 05:47:55 2026 GMT
  host: transcarent.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Transcarent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Transcarent, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Transcarent
provider_slug: transcarent
slug: transcarent-domain-security
source_filename: transcarent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: transcarent.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 05:47:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: transcarent.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transcarent/refs/heads/main/security/transcarent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Health
- Healthcare
- Digital Health
- Benefits Navigation
- Care Navigation
- Virtual Care
- Artificial Intelligence
- Health Benefits
---
