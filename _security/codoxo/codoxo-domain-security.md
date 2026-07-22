---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: codoxo.com
  spf: true
hosts:
- cert_expires: Oct 11 07:26:00 2026 GMT
  host: www.codoxo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codoxo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codoxo, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Codoxo
provider_slug: codoxo
slug: codoxo-domain-security
source_filename: codoxo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.codoxo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 07:26:00 2026 GMT\n  hsts: false\ndomains:\n- domain: codoxo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codoxo/refs/heads/main/security/codoxo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Healthtech
- Healthcare
- Artificial Intelligence
- Fraud Detection
- Payment Integrity
- Machine Learning
- Payers
---
