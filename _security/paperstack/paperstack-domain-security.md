---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: paperstack.ai
  spf: true
hosts:
- cert_expires: Oct  1 07:20:37 2026 GMT
  host: www.paperstack.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Paperstack Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Paperstack, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Paperstack
provider_slug: paperstack
slug: paperstack-domain-security
source_filename: paperstack-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.paperstack.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 07:20:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: paperstack.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paperstack/refs/heads/main/security/paperstack-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Financial Services
- Fintech
- Lending
- Working Capital
- Revenue-Based Financing
- Private Credit
- E-Commerce
- Direct-to-Consumer
- Canada
---
