---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: hw.ac.uk
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: libcal.com
  spf: false
hosts:
- cert_expires: Dec 20 23:59:59 2026 GMT
  host: www.hw.ac.uk
  hsts: true
  hsts_max_age: 15768000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 15:41:21 2026 GMT
  host: researchportal.hw.ac.uk
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 10 12:04:24 2026 GMT
  host: hw.ac.libcal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Heriot Watt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Heriot-Watt University, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Heriot-Watt University
provider_slug: heriot-watt
slug: heriot-watt-domain-security
source_filename: heriot-watt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.hw.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 15768000\n- host: researchportal.hw.ac.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 15:41:21 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: hw.ac.libcal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 12:04:24 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: hw.ac.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: libcal.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/heriot-watt/refs/heads/main/security/heriot-watt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Education
- Higher Education
- University
- Scotland
- United Kingdom
- Research
- Library
- Open Access
---
