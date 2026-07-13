---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: sportdataapi.com
  spf: false
hosts:
- cert_expires: Oct  5 07:13:28 2026 GMT
  host: sportdataapi.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Sport Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Sport Data, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Sport Data
provider_slug: sport-data
slug: sport-data-domain-security
source_filename: sport-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sportdataapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 07:13:28 2026 GMT\n  hsts: null\ndomains:\n- domain: sportdataapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sport-data/refs/heads/main/security/sport-data-domain-security.yml
summary_line: TLSv1.3
tags:
- Sports And Fitness
- Public APIs
---
