---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: honda.com
  spf: true
hosts:
- cert_expires: Jan  8 23:59:59 2027 GMT
  host: www.honda.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 23:59:59 2027 GMT
  host: csat.services.honda.com
  hsts: null
  https: true
  tls_version: TLSv1.2
- cert_expires: Feb  1 23:59:59 2027 GMT
  host: rating.services.honda.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Honda Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Honda, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Honda
provider_slug: honda
slug: honda-domain-security
source_filename: honda-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.honda.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  8 23:59:59 2027 GMT\n  hsts: null\n- host: csat.services.honda.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 23 23:59:59 2027 GMT\n  hsts: null\n- host: rating.services.honda.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Feb  1 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: honda.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honda/refs/heads/main/security/honda-domain-security.yml
summary_line: TLSv1.3
tags:
- Automobiles
- Automotive
- Cars
- Vehicles
---
