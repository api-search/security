---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: zibra.ai
  spf: true
hosts:
- cert_expires: Sep 21 16:32:00 2026 GMT
  host: zibra.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Zibra Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zibra AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Zibra AI
provider_slug: zibra-ai
slug: zibra-ai-domain-security
source_filename: zibra-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zibra.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 16:32:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: zibra.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zibra-ai/refs/heads/main/security/zibra-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Volumetric
- VFX
- 3D Graphics
- Game Development
- Real-Time Rendering
- Compression
- SDK
- OpenVDB
- Unreal Engine
- Houdini
---
