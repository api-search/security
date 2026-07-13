---
description: ''
domains:
- caa:
  - 0 issue "entrust.net"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: icao.int
  spf: true
hosts:
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: www.icao.int
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Mar  2 23:59:59 2027 GMT
  host: applications.icao.int
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Icao Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ICAO, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ICAO
provider_slug: icao
slug: icao-domain-security
source_filename: icao-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.icao.int\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: applications.icao.int\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Mar  2 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: icao.int\n  dnssec: false\n  caa:\n  - 0 issue \"entrust.net\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/icao/refs/heads/main/security/icao-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Airlines
- Airports
- Airspace
- Aviation
- Reference Data
- Standards
- United Nations
---
