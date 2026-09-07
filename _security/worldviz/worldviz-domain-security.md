---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: worldviz.com
  spf: false
hosts:
- cert_expires: Oct 14 07:45:53 2026 GMT
  host: www.worldviz.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Worldviz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WorldViz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: WorldViz
provider_slug: worldviz
slug: worldviz-domain-security
source_filename: worldviz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.worldviz.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 07:45:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: worldviz.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/worldviz/refs/heads/main/security/worldviz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Virtual Reality
- Augmented Reality
- Simulation
- Research
- Training
- 3D Graphics
- Eye Tracking
- Motion Tracking
- Python
- Software
---
