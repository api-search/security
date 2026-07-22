---
api_specs:
- filename: wetravel-partner-openapi.json
  format: json
  label: WeTravel Partner API
  slug: wetravel-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/openapi/wetravel-partner-openapi.json
description: ''
domains:
- caa:
  - 0 issue "amazon.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: wetravel.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: wetravel.to
  spf: true
hosts:
- cert_expires: Sep 10 14:13:36 2026 GMT
  host: www.wetravel.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 10 06:02:04 2026 GMT
  host: api.wetravel.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 19:09:44 2026 GMT
  host: api.demo.wetravel.to
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Wetravel Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for WeTravel, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: WeTravel
provider_slug: wetravel
slug: wetravel-domain-security
source_filename: wetravel-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.wetravel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 10 14:13:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.wetravel.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 10 06:02:04 2026 GMT\n  hsts: null\n- host: api.demo.wetravel.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 19:09:44 2026 GMT\n  hsts: null\ndomains:\n- domain: wetravel.com\n  dnssec: true\n  caa:\n  - 0 issue \"amazon.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: wetravel.to\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wetravel/refs/heads/main/security/wetravel-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Business Applications
- Travel
- Booking
- Payments
- Trip Management
- Tour Operators
- Travel Technology
---
