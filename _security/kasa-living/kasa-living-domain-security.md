---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: kasa.com
  spf: true
hosts:
- cert_expires: Oct 28 15:33:46 2026 GMT
  host: kasa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  8 11:20:56 2026 GMT
  host: stay.kasa.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 22 23:59:59 2027 GMT
  host: help.kasa.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 05:08:46 2026 GMT
  host: blog.kasa.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Kasa Living Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kasa Living, probed live across 4 host(s) and 1 registrable domain(s). 4 host(s) serve HTTPS (up to TLSv1.3); 4 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Kasa Living
provider_slug: kasa-living
slug: kasa-living-domain-security
source_filename: kasa-living-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kasa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 28 15:33:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: stay.kasa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  8 11:20:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: help.kasa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 22 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: blog.kasa.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 05:08:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kasa.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kasa-living/refs/heads/main/security/kasa-living-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Hospitality
- Travel
- Short Term Rental
- Real Estate
- Accommodations
- Property Management
- Corporate Housing
---
