---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: nat.gov.tw
  spf: false
hosts:
- cert_expires: Jan 16 15:59:59 2027 GMT
  host: ncdr.nat.gov.tw
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ncdr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NCDR (Taiwan), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: NCDR (Taiwan)
provider_slug: ncdr
slug: ncdr-domain-security
source_filename: ncdr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ncdr.nat.gov.tw\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 16 15:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: nat.gov.tw\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/ncdr/security/ncdr-domain-security.yml
summary_line: TLSv1.3 · DNSSEC
tags:
- Government
- Disaster Management
- Taiwan
- Public Safety
- Data Services
---
