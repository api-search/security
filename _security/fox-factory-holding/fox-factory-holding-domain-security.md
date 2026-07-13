---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: foxfactory.com
  spf: false
hosts:
- cert_expires: Jan  6 23:16:17 2027 GMT
  host: www.foxfactory.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- host: developer.foxfactory.com
  https: false
- host: api.foxfactory.com
  https: false
kind: domain-security
layout: security
method: probed
name: Fox Factory Holding Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Fox Factory Holding, probed live across 3 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Fox Factory Holding
provider_slug: fox-factory-holding
slug: fox-factory-holding-domain-security
source_filename: fox-factory-holding-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.foxfactory.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  6 23:16:17 2027 GMT\n  hsts: null\n- host: developer.foxfactory.com\n  https: false\n- host: api.foxfactory.com\n  https: false\ndomains:\n- domain: foxfactory.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fox-factory-holding/refs/heads/main/security/fox-factory-holding-domain-security.yml
summary_line: TLSv1.3
tags:
- Suspension
- Cycling
- Powersports
---
