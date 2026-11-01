---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: millnorway.com
  spf: true
hosts:
- cert_expires: Jan 13 15:34:29 2027 GMT
  host: millnorway.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mill Heat Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mill (heaters), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Mill (heaters)
provider_slug: mill-heat
slug: mill-heat-domain-security
source_filename: mill-heat-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: millnorway.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 15:34:29 2027 GMT\n  hsts: false\ndomains:\n- domain: millnorway.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/mill-heat/security/mill-heat-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Heating
- IoT
- ScandinavianDesign
- EnergyEfficiency
---
