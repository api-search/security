---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: teradar.com
  spf: true
hosts:
- cert_expires: Oct 11 14:12:43 2026 GMT
  host: teradar.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Teradar Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Teradar, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Teradar
provider_slug: teradar
slug: teradar-domain-security
source_filename: teradar-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: teradar.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 11 14:12:43 2026 GMT\n  hsts: false\ndomains:\n- domain: teradar.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/teradar/refs/heads/main/security/teradar-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Sensors
- Semiconductors
- Terahertz
- Automotive
- Autonomous Vehicles
- Radar
- LiDAR
- Perception
- Defense
- Hardware
---
