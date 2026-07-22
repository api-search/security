---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: akashx.ai
  spf: false
hosts:
- cert_expires: Oct  9 05:00:44 2026 GMT
  host: akashx.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akashx Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AkashX, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: AkashX
provider_slug: akashx
slug: akashx-domain-security
source_filename: akashx-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: akashx.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 05:00:44 2026 GMT\n  hsts: false\ndomains:\n- domain: akashx.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akashx/refs/heads/main/security/akashx-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Artificial Intelligence
- Data
- Database
- Analytics
- SQL
- Lakehouse
- Machine Learning
---
