---
api_specs:
- filename: ncr-voyix-platform-openapi.yml
  format: yaml
  label: NCR Voyix Commerce Platform APIs (Aloha)
  slug: ncr-voyix-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aloha-pos/refs/heads/main/openapi/ncr-voyix-platform-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ncrvoyix.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: ncr.com
  spf: true
hosts:
- cert_expires: Feb  3 23:59:59 2027 GMT
  host: www.ncrvoyix.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: developer.ncrvoyix.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 24 23:59:59 2026 GMT
  host: api.ncr.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Aloha Pos Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aloha POS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Aloha POS
provider_slug: aloha-pos
slug: aloha-pos-domain-security
source_filename: aloha-pos-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ncrvoyix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.ncrvoyix.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: false\n- host: api.ncr.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 24 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: ncrvoyix.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: ncr.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aloha-pos/refs/heads/main/security/aloha-pos-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- POS
- Restaurant
- Hospitality
- NCR
---
