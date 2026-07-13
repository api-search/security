---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: aihabitat.org
  spf: true
hosts:
- cert_expires: Aug 26 20:40:33 2026 GMT
  host: aihabitat.org
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Habitat Lab Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Habitat Lab, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Habitat Lab
provider_slug: habitat-lab
slug: habitat-lab-domain-security
source_filename: habitat-lab-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aihabitat.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 20:40:33 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: aihabitat.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/habitat-lab/refs/heads/main/security/habitat-lab-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Artificial Intelligence
- Embodied AI
- Research
- Robotics
- Simulation
---
