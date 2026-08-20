---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dyna.co
  spf: true
hosts:
- cert_expires: Oct 24 08:35:59 2026 GMT
  host: www.dyna.co
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dyna Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dyna Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Dyna Robotics
provider_slug: dyna-robotics
slug: dyna-robotics-domain-security
source_filename: dyna-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dyna.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 24 08:35:59 2026 GMT\n  hsts: null\ndomains:\n- domain: dyna.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dyna-robotics/refs/heads/main/security/dyna-robotics-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Robotics
- Artificial Intelligence
- Machine-Learning
- Foundation Models
- Automation
- Manufacturing
- Embodied AI
- Robotics as a Service
---
