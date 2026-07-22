---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: melon.sa
  spf: true
hosts:
- cert_expires: Aug 24 17:36:59 2026 GMT
  host: melon.sa
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Melon Digital Insurance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Melon Digital Insurance, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Melon Digital Insurance
provider_slug: melon-digital-insurance
slug: melon-digital-insurance-domain-security
source_filename: melon-digital-insurance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: melon.sa\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 17:36:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: melon.sa\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/melon-digital-insurance/refs/heads/main/security/melon-digital-insurance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Insurance
- Insurtech
- Digital Insurance
- Saudi Arabia
- Fintech
- Artificial Intelligence
---
