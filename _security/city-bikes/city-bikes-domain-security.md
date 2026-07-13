---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: citybik.es
  spf: true
hosts:
- cert_expires: Aug 28 18:09:11 2026 GMT
  host: api.citybik.es
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: City Bikes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for City Bikes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: City Bikes
provider_slug: city-bikes
slug: city-bikes-domain-security
source_filename: city-bikes-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.citybik.es\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 28 18:09:11 2026 GMT\n  hsts: false\ndomains:\n- domain: citybik.es\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/city-bikes/refs/heads/main/security/city-bikes-domain-security.yml
summary_line: TLSv1.3
tags:
- Sports And Fitness
- Public APIs
---
