---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moonlakeai.com
  spf: true
hosts:
- cert_expires: Oct 14 06:17:26 2026 GMT
  host: moonlakeai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: app.moonlakeai.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Moonlake Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MoonLake AI, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MoonLake AI
provider_slug: moonlake-ai
slug: moonlake-ai-domain-security
source_filename: moonlake-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: moonlakeai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 06:17:26 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.moonlakeai.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: moonlakeai.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moonlake-ai/refs/heads/main/security/moonlake-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- World Models
- Simulation
- Embodied AI
- Robotics
- 3D Generation
- Digital Twins
- Synthetic Data
---
