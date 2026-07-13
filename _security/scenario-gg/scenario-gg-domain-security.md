---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: scenario.com
  spf: true
hosts:
- cert_expires: Oct  4 17:45:00 2026 GMT
  host: www.scenario.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 14 04:18:30 2026 GMT
  host: app.scenario.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 17:17:08 2026 GMT
  host: docs.scenario.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Scenario Gg Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Scenario, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Scenario
provider_slug: scenario-gg
slug: scenario-gg-domain-security
source_filename: scenario-gg-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.scenario.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 17:45:00 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: app.scenario.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 14 04:18:30 2026 GMT\n  hsts: null\n- host: docs.scenario.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 17:17:08 2026 GMT\n  hsts: false\ndomains:\n- domain: scenario.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scenario-gg/refs/heads/main/security/scenario-gg-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Artificial Intelligence
- Game Assets
- Game Development
- Generative AI
- Image Generation
- Video Generation
- Audio Generation
- 3D Assets
- Custom Model Training
- LoRA
- ControlNet
- Creative AI
- Asset Pipeline
---
