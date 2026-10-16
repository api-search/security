---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: axio.co.in
  spf: true
hosts:
- cert_expires: Nov  7 02:31:56 2026 GMT
  host: www.axio.co.in
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Capitalfloat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Capitalfloat, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Capitalfloat
provider_slug: capitalfloat
slug: capitalfloat-domain-security
source_filename: capitalfloat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.axio.co.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  7 02:31:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: axio.co.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capitalfloat/refs/heads/main/security/capitalfloat-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Finance
- FinTech
- ConsumerFinance
- India
- Payments
---
