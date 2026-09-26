---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: anyword.com
  spf: true
hosts:
- cert_expires: Nov  9 22:39:21 2026 GMT
  host: www.anyword.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Anyword Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Anyword, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Anyword
provider_slug: anyword
slug: anyword-domain-security
source_filename: anyword-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anyword.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 22:39:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anyword.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anyword/refs/heads/main/security/anyword-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Content Generation
- Marketing
- SaaS
---
