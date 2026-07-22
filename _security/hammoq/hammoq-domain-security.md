---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: hammoq.com
  spf: true
hosts:
- cert_expires: Sep  8 12:54:23 2026 GMT
  host: hammoq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hammoq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hammoq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Hammoq
provider_slug: hammoq
slug: hammoq-domain-security
source_filename: hammoq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hammoq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 12:54:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: hammoq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hammoq/refs/heads/main/security/hammoq-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Ai
- Recommerce
- Resale
- Ecommerce
- Marketplace
- Machine Vision
- Generative AI
- Automation
- Retail Returns
---
