---
api_specs:
- filename: v4.json
  format: json
  label: Bitly API v4
  slug: bitly-api
  spec_type: OpenAPI
  url: https://dev.bitly.com/v4/v4.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issuewild "amazon.com"
  - 0 iodef "mailto:abuse@bit.ly"
  - 0 issue "amazon.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: bitly.com
  spf: true
hosts:
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: bitly.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  5 23:59:59 2026 GMT
  host: dev.bitly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: api-ssl.bitly.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Bitly Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bitly, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Bitly
provider_slug: bitly
slug: bitly-domain-security
source_filename: bitly-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bitly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: null\n- host: dev.bitly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  5 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-ssl.bitly.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: bitly.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issuewild \"amazon.com\"\n  - 0 iodef \"mailto:abuse@bit.ly\"\n  - 0 issue \"amazon.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bitly/refs/heads/main/security/bitly-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Links
- URL Shortener
- QR Codes
- Analytics
- Marketing
---
