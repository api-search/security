---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: akara.ai
  spf: true
hosts:
- cert_expires: Aug 28 02:27:43 2026 GMT
  host: akara.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akara Robotics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akara Robotics, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Akara Robotics
provider_slug: akara-robotics
slug: akara-robotics-domain-security
source_filename: akara-robotics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: akara.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 02:27:43 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: akara.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akara-robotics/refs/heads/main/security/akara-robotics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Robotics
- Healthcare
- Automation
- Artificial Intelligence
- Hospitals
- Disinfection
- Medical Devices
---
