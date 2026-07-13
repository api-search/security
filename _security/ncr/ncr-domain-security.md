---
api_specs:
- filename: ncr-voyix-commerce-platform-openapi.yml
  format: yaml
  label: NCR Voyix Commerce Platform APIs
  slug: ncr-voyix-commerce-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ncr/refs/heads/main/openapi/ncr-voyix-commerce-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ncr.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ncrvoyix.com
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.ncr.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.ncrvoyix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 21 09:47:56 2026 GMT
  host: www.ncratleos.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ncr Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NCR, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NCR
provider_slug: ncr
slug: ncr-domain-security
source_filename: ncr-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ncr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ncrvoyix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: www.ncratleos.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 21 09:47:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: ncr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ncrvoyix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ncr/refs/heads/main/security/ncr-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Retail
- Banking
- ATM
- Point of Sale
- Commerce
- Fortune 500
---
