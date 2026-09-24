---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: hiive.com
  spf: true
hosts:
- cert_expires: Dec 14 14:19:32 2026 GMT
  host: www.hiive.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Alpian Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Alpian, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Alpian
provider_slug: alpian
slug: alpian-domain-security
source_filename: alpian-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-24'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hiive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 14:19:32 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hiive.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alpian/refs/heads/main/security/alpian-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Banking
- Savings
- Investing
- Pillar 3a
- Multi‑currency
- Debit card
- Neobank
---
