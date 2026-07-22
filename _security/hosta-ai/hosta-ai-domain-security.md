---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: hosta.ai
  spf: true
hosts:
- cert_expires: Oct 12 16:36:33 2026 GMT
  host: hosta.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Hosta Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Hosta a.i., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Hosta a.i.
provider_slug: hosta-ai
slug: hosta-ai-domain-security
source_filename: hosta-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: hosta.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 12 16:36:33 2026 GMT\n  hsts: false\ndomains:\n- domain: hosta.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hosta-ai/refs/heads/main/security/hosta-ai-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Property Technology
- PropTech
- Artificial Intelligence
- Computer Vision
- Property Assessment
- Insurance
- Construction
- Real Estate
- Spatial Analytics
---
