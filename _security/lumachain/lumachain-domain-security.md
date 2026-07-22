---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lumachain.io
  spf: true
hosts:
- cert_expires: Oct 16 00:52:35 2026 GMT
  host: lumachain.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lumachain Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lumachain, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Lumachain
provider_slug: lumachain
slug: lumachain-domain-security
source_filename: lumachain-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lumachain.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 00:52:35 2026 GMT\n  hsts: false\ndomains:\n- domain: lumachain.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lumachain/refs/heads/main/security/lumachain-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Deep Tech
- Artificial Intelligence
- Computer Vision
- Food Supply Chain
- Food Safety
- Traceability
- Manufacturing
---
