---
api_specs:
- filename: progressive-auto-quote-api-openapi.yml
  format: yaml
  label: Progressive Auto Quote API
  slug: auto-quote-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/progressive/refs/heads/main/openapi/progressive-auto-quote-api-openapi.yml
- filename: progressive-certificate-of-insurance-api-openapi.yml
  format: yaml
  label: Progressive Certificate of Insurance API
  slug: certificate-of-insurance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/progressive/refs/heads/main/openapi/progressive-certificate-of-insurance-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: progressive.com
  spf: true
hosts:
- cert_expires: Feb 25 23:59:59 2027 GMT
  host: developer.progressive.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 19 23:59:59 2026 GMT
  host: www.progressive.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 13 23:59:59 2026 GMT
  host: api.progressive.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Progressive Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Progressive, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Progressive
provider_slug: progressive
slug: progressive-domain-security
source_filename: progressive-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: developer.progressive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 25 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.progressive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 19 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.progressive.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 13 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: progressive.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/progressive/refs/heads/main/security/progressive-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Auto Insurance
- Commercial Insurance
- Embedded Insurance
- Insurance
- Quoting
- Fortune 500
---
