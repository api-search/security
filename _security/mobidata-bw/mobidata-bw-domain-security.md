---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: mobidata-bw.de
  spf: false
hosts:
- cert_expires: Mar 29 14:20:50 2027 GMT
  host: mobidata-bw.de
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: MobiData BW Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MobiData BW, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: MobiData BW
provider_slug: mobidata-bw
slug: mobidata-bw-domain-security
source_filename: mobidata-bw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-16'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mobidata-bw.de\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 29 14:20:50 2027 GMT\n  hsts: false\ndomains:\n- domain: mobidata-bw.de\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/mobidata-bw/security/mobidata-bw-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Mobility
- Open Data
- Transportation
- Germany
---
