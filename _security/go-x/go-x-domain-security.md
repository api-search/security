---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: goxapp.com
  spf: true
hosts:
- cert_expires: Jan 10 23:59:59 2027 GMT
  host: goxapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Go X Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Go X, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Go X
provider_slug: go-x
slug: go-x-domain-security
source_filename: go-x-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: goxapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: goxapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/go-x/refs/heads/main/security/go-x-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Micromobility
- Electric Scooters
- Scooter Sharing
- E-Bikes
- Mobility
- Transportation
- Vehicle Rental
---
