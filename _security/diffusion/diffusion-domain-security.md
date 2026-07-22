---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: diffusionsoftware.com
  spf: true
hosts:
- cert_expires: Sep  1 11:52:46 2026 GMT
  host: www.diffusionsoftware.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Diffusion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Diffusion, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Diffusion
provider_slug: diffusion
slug: diffusion-domain-security
source_filename: diffusion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.diffusionsoftware.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  1 11:52:46 2026 GMT\n  hsts: false\ndomains:\n- domain: diffusionsoftware.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diffusion/refs/heads/main/security/diffusion-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Company
- Radio Data System
- RDS Encoder
- RBDS
- FM Radio
- Radio Broadcast
- Broadcast Software
- Audio Encoding
- RadioText
- Windows Software
---
