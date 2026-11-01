---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: lg.com
  spf: true
hosts:
- cert_expires: Jan  3 23:59:59 2027 GMT
  host: lg.com
  hsts: null
  https: true
  tls_version: TLSv1.2
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Lg Electronics Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for LG ThinQ, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.2); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: LG ThinQ
provider_slug: lg-electronics
slug: lg-electronics-domain-security
source_filename: lg-electronics-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lg.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan  3 23:59:59 2027 GMT\n  hsts: null\ndomains:\n- domain: lg.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/lg-electronics/security/lg-electronics-domain-security.yml
summary_line: TLSv1.2 · DMARC
tags:
- Company
- SmartHome
- IoT
- ConsumerElectronics
- AI
---
