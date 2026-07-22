---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: philon.ai
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: philon.ai
  hsts: true
  hsts_max_age: 10886400
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Philon Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Philon, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Philon
provider_slug: philon
slug: philon-domain-security
source_filename: philon-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: philon.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 10886400\ndomains:\n- domain: philon.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/philon/refs/heads/main/security/philon-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Robotics
- Artificial Intelligence
- Research
- Open Source
- Humanoid Robots
- Foundation Models
- Embodied AI
---
