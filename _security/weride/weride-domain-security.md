---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: weride.ai
  spf: true
hosts:
- cert_expires: Nov 22 00:07:46 2026 GMT
  host: weride.ai
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Weride Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeRide, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: WeRide
provider_slug: weride
slug: weride-domain-security
source_filename: weride-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: weride.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 22 00:07:46 2026 GMT\n  hsts: false\ndomains:\n- domain: weride.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weride/refs/heads/main/security/weride-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Autonomous Driving
- Robotaxi
- Self-Driving
- Mobility
- Transportation
- ADAS
- Logistics
---
