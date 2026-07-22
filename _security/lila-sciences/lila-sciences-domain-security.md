---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lila.ai
  spf: true
hosts:
- cert_expires: Oct 10 19:16:35 2026 GMT
  host: www.lila.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lila Sciences Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lila Sciences, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lila Sciences
provider_slug: lila-sciences
slug: lila-sciences-domain-security
source_filename: lila-sciences-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.lila.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 19:16:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lila.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lila-sciences/refs/heads/main/security/lila-sciences-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Scientific Research
- Life Sciences
- Biotechnology
- Therapeutics
- Advanced Materials
- Laboratory Automation
- Robotics
- Drug Discovery
- Energy
---
