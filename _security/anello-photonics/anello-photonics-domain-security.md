---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: anellophotonics.com
  spf: true
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: readthedocs.io
  spf: false
hosts:
- cert_expires: Oct 13 09:41:19 2026 GMT
  host: www.anellophotonics.com
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 25 13:31:53 2026 GMT
  host: docs-a1.readthedocs.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Anello Photonics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ANELLO Photonics, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: ANELLO Photonics
provider_slug: anello-photonics
slug: anello-photonics-domain-security
source_filename: anello-photonics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.anellophotonics.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 13 09:41:19 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: docs-a1.readthedocs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 13:31:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: anellophotonics.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: readthedocs.io\n  dnssec: false\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"amazonaws.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anello-photonics/refs/heads/main/security/anello-photonics-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Inertial Navigation
- Optical Gyroscope
- Silicon Photonics
- GNSS
- GPS-Denied Navigation
- Sensors
- Robotics
- Defense
- Autonomous Vehicles
- Embedded Systems
- IMU
---
