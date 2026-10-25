---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: fctgl.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tpconnects.com
  spf: true
hosts:
- cert_expires: Dec 12 16:06:26 2026 GMT
  host: www.fctgl.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 21 02:44:47 2026 GMT
  host: tpconnects.com
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Flight Centre Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Flight Centre Travel Group, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Flight Centre Travel Group
provider_slug: flight-centre
slug: flight-centre-domain-security
source_filename: flight-centre-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.fctgl.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 12 16:06:26 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: tpconnects.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 02:44:47 2026 GMT\n  hsts: false\ndomains:\n- domain: fctgl.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: tpconnects.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flight-centre/refs/heads/main/security/flight-centre-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Australia
- Corporate Travel
- Travel Agency
- Distribution
- NDC
- Aviation
- Booking
- Hotels
- Aggregator
---
