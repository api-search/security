---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: netcad.com.tr
  spf: true
hosts:
- cert_expires: Nov 10 21:15:49 2026 GMT
  host: www.netcad.com.tr
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Netcad Yazilim A S Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NETCAD YAZILIM A.S., probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: NETCAD YAZILIM A.S.
provider_slug: netcad-yazilim-a-s
slug: netcad-yazilim-a-s-domain-security
source_filename: netcad-yazilim-a-s-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.netcad.com.tr\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 10 21:15:49 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: netcad.com.tr\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/netcad-yazilim-a-s/security/netcad-yazilim-a-s-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- GIS
- Mapping
- Smart-City
- Cadastral
---
