---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: generalistai.com
  spf: true
hosts:
- cert_expires: Sep 30 05:42:45 2026 GMT
  host: generalistai.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Generalist Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Generalist AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Generalist AI
provider_slug: generalist-ai
slug: generalist-ai-domain-security
source_filename: generalist-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: generalistai.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 30 05:42:45 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: generalistai.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/generalist-ai/refs/heads/main/security/generalist-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Artificial Intelligence
- Robotics
- Foundation Models
- Physical AI
- Embodied AI
- Robot Learning
- Machine Learning
---
