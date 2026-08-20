---
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: savills.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: savills.co.uk
  spf: true
hosts:
- cert_expires: Jan 27 23:59:59 2027 GMT
  host: www.savills.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: www.savills.co.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb 24 23:59:59 2027 GMT
  host: www.savills.us
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Savills Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Savills, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Savills
provider_slug: savills
slug: savills-domain-security
source_filename: savills-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.savills.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.savills.co.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.savills.us\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: savills.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: savills.co.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/savills/refs/heads/main/security/savills-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Real-Estate
- United Kingdom
- Commercial Real Estate
- Property Listings
- Valuation
- Property Management
- Brokerage
- Rentals
- PropTech
- Investment Management
---
