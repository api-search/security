---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: motorq.com
  spf: true
hosts:
- cert_expires: Oct  2 08:50:52 2026 GMT
  host: motorq.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Motorq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Motorq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Motorq
provider_slug: motorq
slug: motorq-domain-security
source_filename: motorq-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: motorq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 08:50:52 2026 GMT\n  hsts: false\ndomains:\n- domain: motorq.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/motorq/refs/heads/main/security/motorq-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Connected Vehicles
- Telematics
- Fleet Management
- Automotive
- Vehicle Data
- Mobility
- IoT
- Insight Partners Portfolio
---
