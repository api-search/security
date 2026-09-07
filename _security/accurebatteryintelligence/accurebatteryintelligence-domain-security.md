---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: accure.net
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: accure-platform.com
  spf: false
hosts:
- cert_expires: Nov  9 18:24:04 2026 GMT
  host: www.accure.net
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: accure-platform.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: gateway.accure-platform.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Accurebatteryintelligence Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ACCURE Battery Intelligence, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: ACCURE Battery Intelligence
provider_slug: accurebatteryintelligence
slug: accurebatteryintelligence-domain-security
source_filename: accurebatteryintelligence-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.accure.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  9 18:24:04 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: accure-platform.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: gateway.accure-platform.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: accure.net\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: accure-platform.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accurebatteryintelligence/refs/heads/main/security/accurebatteryintelligence-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Energy
- Battery
- Energy Storage
- Analytics
- Artificial Intelligence
- Internet of Things
- Electric Vehicles
- Germany
---
