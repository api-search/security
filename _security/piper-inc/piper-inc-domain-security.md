---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: playpiper.in
  spf: true
hosts:
- cert_expires: Sep  4 15:40:33 2026 GMT
  host: playpiper.in
  hsts: true
  hsts_max_age: 7889238
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Piper Inc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Piper Inc., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Piper Inc.
provider_slug: piper-inc
slug: piper-inc-domain-security
source_filename: piper-inc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: playpiper.in\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 15:40:33 2026 GMT\n  hsts: true\n  hsts_max_age: 7889238\ndomains:\n- domain: playpiper.in\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/piper-inc/refs/heads/main/security/piper-inc-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Education
- EdTech
- STEM
- Hardware
- E-Commerce
- Agentic Commerce
- MCP
- Shopify
---
