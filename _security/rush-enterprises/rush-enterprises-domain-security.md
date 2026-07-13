---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: rushenterprises.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: rushtruckcenters.com
  spf: true
hosts:
- cert_expires: Jul 27 19:30:44 2026 GMT
  host: www.rushenterprises.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 27 19:30:44 2026 GMT
  host: www.rushtruckcenters.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 22:42:22 2026 GMT
  host: serviceconnect.rushcare.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Rush Enterprises Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Rush Enterprises, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Rush Enterprises
provider_slug: rush-enterprises
slug: rush-enterprises-domain-security
source_filename: rush-enterprises-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.rushenterprises.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 27 19:30:44 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: www.rushtruckcenters.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 27 19:30:44 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: serviceconnect.rushcare.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 22:42:22 2026 GMT\n  hsts: false\ndomains:\n- domain: rushenterprises.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: rushtruckcenters.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rush-enterprises/refs/heads/main/security/rush-enterprises-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Commercial Vehicles
- Fleet Management
- Telematics
- Truck Dealerships
- Transportation
- Fortune 1000
---
