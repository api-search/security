---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rome2rio.com
  spf: true
hosts:
- cert_expires: Feb  5 23:59:59 2027 GMT
  host: www.rome2rio.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: free.rome2rio.com
  https: false
kind: domain-security
layout: security
method: probed
name: Rome2Rio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rome2Rio, probed live across 2 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Rome2Rio
provider_slug: rome2rio
slug: rome2rio-domain-security
source_filename: rome2rio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rome2rio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  5 23:59:59 2027 GMT\n  hsts: false\n- host: free.rome2rio.com\n  https: false\ndomains:\n- domain: rome2rio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rome2rio/refs/heads/main/security/rome2rio-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Travel
- Multi-Modal
- Transportation
- Routes
- Transit
- Flights
- Trains
- Buses
- Ferries
- Navigation
---
