---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: wandercraft.eu
  spf: true
hosts:
- cert_expires: Oct 10 17:33:44 2026 GMT
  host: en.wandercraft.eu
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Wandercraft Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Wandercraft, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Wandercraft
provider_slug: wandercraft
slug: wandercraft-domain-security
source_filename: wandercraft-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: en.wandercraft.eu\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 17:33:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: wandercraft.eu\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wandercraft/refs/heads/main/security/wandercraft-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Robotics
- Exoskeleton
- Humanoid Robots
- Medical Devices
- Rehabilitation
- Healthcare
- Physical AI
- Industrial Automation
- Mobility
- Assistive Technology
- Deep Tech
- France
---
