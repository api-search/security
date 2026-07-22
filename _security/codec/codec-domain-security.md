---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: codec.ai
  spf: true
hosts:
- cert_expires: Sep 30 01:45:06 2026 GMT
  host: codec.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Codec Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Codec, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Codec
provider_slug: codec
slug: codec-domain-security
source_filename: codec-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: codec.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 01:45:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: codec.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codec/refs/heads/main/security/codec-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Audience Intelligence
- Marketing
- Community
- Brand Strategy
- Consulting
---
