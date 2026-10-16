---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bwsensing.com
  spf: true
hosts:
- cert_expires: Oct 29 06:10:58 2026 GMT
  host: www.bwsensing.com
  hsts: false
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bwsensing Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bwsensing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bwsensing
provider_slug: bwsensing
slug: bwsensing-domain-security
source_filename: bwsensing-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bwsensing.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 06:10:58 2026 GMT\n  hsts: false\ndomains:\n- domain: bwsensing.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bwsensing/refs/heads/main/security/bwsensing-domain-security.yml
summary_line: TLSv1.2
tags:
- Sensor
- Inertial Measurement
- IoT
- Industrial
- Construction
---
