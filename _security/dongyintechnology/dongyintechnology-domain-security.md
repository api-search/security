---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: doyin.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: equityzen.com
  spf: true
hosts:
- cert_expires: Jan  7 23:59:59 2027 GMT
  host: www.doyin.com
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb 11 23:59:59 2027 GMT
  host: equityzen.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Dongyintechnology Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Dongyintechnology, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Dongyintechnology
provider_slug: dongyintechnology
slug: dongyintechnology-domain-security
source_filename: dongyintechnology-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.doyin.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  7 23:59:59 2027 GMT\n  hsts: false\n- host: equityzen.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: doyin.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: equityzen.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/dongyintechnology/security/dongyintechnology-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Supply Chain
- Software-as-a-Service
- Digital Solutions
- China
- Manufacturing
- Pumps
---
