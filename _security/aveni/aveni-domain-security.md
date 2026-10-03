---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aveni.ai
  spf: true
hosts:
- cert_expires: Mar 30 23:59:59 2027 GMT
  host: aveni.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aveni Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aveni, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aveni
provider_slug: aveni
slug: aveni-domain-security
source_filename: aveni-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aveni.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 30 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aveni.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aveni/refs/heads/main/security/aveni-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Fintech
- RegTech
- Artificial Intelligence
- Financial Services
- Edinburgh
---
