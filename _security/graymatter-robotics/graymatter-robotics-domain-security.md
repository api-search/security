---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: graymatter-robotics.com
  spf: true
hosts:
- cert_expires: Oct  8 04:17:42 2026 GMT
  host: graymatter-robotics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 20:29:43 2026 GMT
  host: factory.graymatter-robotics.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Graymatter Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GrayMatter Robotics, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GrayMatter Robotics
provider_slug: graymatter-robotics
slug: graymatter-robotics-domain-security
source_filename: graymatter-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: graymatter-robotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 04:17:42 2026 GMT\n  hsts: null\n- host: factory.graymatter-robotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 20:29:43 2026 GMT\n  hsts: null\ndomains:\n- domain: graymatter-robotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/graymatter-robotics/refs/heads/main/security/graymatter-robotics-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Robotics
- Industrial Robotics
- Manufacturing
- Automation
- Artificial Intelligence
- Physical AI
- Machine Vision
- Surface Finishing
- Sanding
- Aerospace
- Defense
- Heavy Equipment
- Robots-as-a-Service
- Factory Automation
---
