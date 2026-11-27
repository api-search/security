---
description: ''
domains:
- caa:
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: daischsensor.com
  spf: true
hosts:
- cert_expires: Dec 12 23:52:01 2026 GMT
  host: daischsensor.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: DAISCH Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for DAISCH, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: DAISCH
provider_slug: daisch
slug: daisch-domain-security
source_filename: daisch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: daischsensor.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 23:52:01 2026 GMT\n  hsts: false\ndomains:\n- domain: daischsensor.com\n  dnssec: true\n  caa:\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/daisch/security/daisch-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- IMU
- Inertial Measurement Unit
- GNSS/INS
- AHRS
- Motion Sensing
- Autonomous Driving
- ADAS
- Robotics
- Sensors
- Hardware Manufacturer
---
