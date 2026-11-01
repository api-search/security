---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: worlddataapi.com
  spf: true
hosts:
- cert_expires: Nov 27 11:33:09 2026 GMT
  host: worlddataapi.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Worlddataapi Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for World Data API, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: World Data API
provider_slug: worlddataapi
slug: worlddataapi-domain-security
source_filename: worlddataapi-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: worlddataapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 27 11:33:09 2026 GMT\n  hsts: false\ndomains:\n- domain: worlddataapi.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/worlddataapi/security/worlddataapi-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Data
- Geography
- Travel
---
