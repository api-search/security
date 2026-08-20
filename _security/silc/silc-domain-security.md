---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: silc.com
  spf: true
hosts:
- cert_expires: Oct  9 04:49:47 2026 GMT
  host: silc.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Silc Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SiLC, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: SiLC
provider_slug: silc
slug: silc-domain-security
source_filename: silc-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: silc.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 04:49:47 2026 GMT\n  hsts: false\ndomains:\n- domain: silc.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silc/refs/heads/main/security/silc-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Silicon Photonics
- LiDAR
- Machine Vision
- Sensors
- Semiconductors
- Robotics
- Perimeter Security
- Computer-Vision
- Hardware
---
