---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: loc8id.com
  spf: true
hosts:
- cert_expires: Jan 22 07:57:34 2027 GMT
  host: loc8id.com
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Loc8ID Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Loc8ID, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Loc8ID
provider_slug: loc8id-com
slug: loc8id-com-domain-security
source_filename: loc8id-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: loc8id.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 22 07:57:34 2027 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: loc8id.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/loc8id-com/security/loc8id-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Short Codes
- GPS Precision
- Real Estate
- Deliveries
- Event
- Field Service Management
- Travel & Tourism
---
