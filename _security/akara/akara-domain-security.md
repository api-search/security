---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: akara.ai
  spf: true
hosts:
- cert_expires: Sep  5 06:13:19 2026 GMT
  host: www.akara.ai
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akara Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akara, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC absent.'
provider_name: Akara
provider_slug: akara
slug: akara-domain-security
source_filename: akara-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.akara.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 06:13:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: akara.ai\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akara/refs/heads/main/security/akara-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Company
- Healthcare
- Robotics
- Artificial Intelligence
- Operating Room
- Automation
- Disinfection
- Computer Vision
- MedTech
---
