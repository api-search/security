---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: dataarobotics.com
  spf: true
hosts:
- cert_expires: Sep  9 11:59:59 2026 GMT
  host: www.dataarobotics.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- host: harix.dataarobotics.com
  https: false
kind: domain-security
layout: security
method: probed
name: Cloudminds Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudMinds, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: CloudMinds
provider_slug: cloudminds
slug: cloudminds-domain-security
source_filename: cloudminds-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-10'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.dataarobotics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 11:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: harix.dataarobotics.com\n  https: false\ndomains:\n- domain: dataarobotics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudminds/refs/heads/main/security/cloudminds-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Frontier Tech
- Robotics
- Cloud Robotics
- Artificial Intelligence
- Robot Development Kit
- HARIX
- gRPC
- Protobuf
- Robot Operating System
- Computer Vision
- Speech Recognition
---
