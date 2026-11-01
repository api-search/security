---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: true
  domain: govt.nz
  spf: false
hosts:
- cert_expires: Mar 24 23:59:59 2027 GMT
  host: www.linz.govt.nz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Land Information New Zealand Linz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Land Information New Zealand (LINZ), probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF absent, DMARC absent.'
provider_name: Land Information New Zealand (LINZ)
provider_slug: land-information-new-zealand-linz
slug: land-information-new-zealand-linz-domain-security
source_filename: land-information-new-zealand-linz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-23'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.linz.govt.nz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: govt.nz\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/land-information-new-zealand-linz/security/land-information-new-zealand-linz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC
tags:
- Property information
- Crown land management
- Overseas investment regulation
- Land registration
- Geospatial data
- Mapping
---
