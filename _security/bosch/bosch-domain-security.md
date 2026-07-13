---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: bosch.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: bosch-iot-suite.com
  spf: false
hosts:
- cert_expires: Jan 22 23:59:59 2027 GMT
  host: www.bosch.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 14:24:57 2026 GMT
  host: bosch-iot-suite.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bosch Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bosch, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Bosch
provider_slug: bosch
slug: bosch-domain-security
source_filename: bosch-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.bosch.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: bosch-iot-suite.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 14:24:57 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bosch.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: bosch-iot-suite.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bosch/refs/heads/main/security/bosch-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Manufacturing
- Automotive
- Industrial
- Technology
- IoT
- Smart Home
---
