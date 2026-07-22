---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: uthana.com
  spf: true
hosts:
- cert_expires: Aug 16 17:56:40 2026 GMT
  host: uthana.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Uthana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Uthana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Uthana
provider_slug: uthana
slug: uthana-domain-security
source_filename: uthana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: uthana.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 17:56:40 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: uthana.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uthana/refs/heads/main/security/uthana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Animation
- 3D Characters
- Generative AI
- Motion Capture
- Gaming
- Robotics
- Foundation Models
- GraphQL
---
