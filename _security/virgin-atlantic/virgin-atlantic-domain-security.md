---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: virginatlantic.com
  spf: true
hosts:
- cert_expires: Oct 31 10:22:41 2026 GMT
  host: www.virginatlantic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  4 12:14:52 2026 GMT
  host: ndc.virginatlantic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Virgin Atlantic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Virgin Atlantic, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Virgin Atlantic
provider_slug: virgin-atlantic
slug: virgin-atlantic-domain-security
source_filename: virgin-atlantic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.virginatlantic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 31 10:22:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ndc.virginatlantic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  4 12:14:52 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: virginatlantic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/virgin-atlantic/refs/heads/main/security/virgin-atlantic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- United Kingdom
- Aviation
- Airline
- Distribution
- NDC
- Booking
- GDS
---
