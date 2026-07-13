---
api_specs:
- filename: abstractapi-phone-openapi.yml
  format: yaml
  label: Abstract API Phone Validation API
  slug: abstractapi-phone-validation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/abstractapi-phone/refs/heads/main/openapi/abstractapi-phone-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: abstractapi.com
  spf: false
hosts:
- cert_expires: Sep 19 20:00:37 2026 GMT
  cert_not_before: Jun 21 20:00:38 2026 GMT
  host: abstractapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: cloudflare
  tls_version: TLSv1.3
  x_frame_options: SAMEORIGIN
- cert_expires: Sep 10 07:12:58 2026 GMT
  cert_not_before: Jun 12 06:13:04 2026 GMT
  host: www.abstractapi.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  server: cloudflare
  tls_version: TLSv1.3
  x_frame_options: SAMEORIGIN
- allow_methods: GET, HEAD, OPTIONS
  cert_expires: Mar 16 23:59:59 2027 GMT
  cert_not_before: Feb 16 00:00:00 2026 GMT
  host: phonevalidation.abstractapi.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  referrer_policy: same-origin
  server: nginx/1.18.0 (Ubuntu)
  tls_version: TLSv1.2
  x_content_type_options: nosniff
  x_frame_options: DENY
kind: domain-security
layout: security
method: probed
name: Abstractapi Phone Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Abstract API Phone Validation, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=none).'
provider_name: Abstract API Phone Validation
provider_slug: abstractapi-phone
slug: abstractapi-phone-domain-security
source_filename: abstractapi-phone-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: abstractapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_not_before: Jun 21 20:00:38 2026 GMT\n  cert_expires: Sep 19 20:00:37 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  server: cloudflare\n  x_frame_options: SAMEORIGIN\n- host: www.abstractapi.com\n  https: true\n  tls_version: TLSv1.3\n  cert_not_before: Jun 12 06:13:04 2026 GMT\n  cert_expires: Sep 10 07:12:58 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  server: cloudflare\n  x_frame_options: SAMEORIGIN\n- host: phonevalidation.abstractapi.com\n  https: true\n  tls_version: TLSv1.2\n  cert_not_before: Feb 16 00:00:00 2026 GMT\n  cert_expires: Mar 16 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n  server: nginx/1.18.0 (Ubuntu)\n  x_frame_options: DENY\n  x_content_type_options: nosniff\n  referrer_policy: same-origin\n  allow_methods: GET,\
  \ HEAD, OPTIONS\ndomains:\n- domain: abstractapi.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: none\nnotes: >-\n  Marketing/docs hosts (abstractapi.com, www.abstractapi.com) sit behind\n  Cloudflare on TLSv1.3 with HSTS. The API host\n  (phonevalidation.abstractapi.com) is served directly by nginx/1.18.0 on\n  TLSv1.2 with HSTS (includeSubDomains), X-Frame-Options DENY,\n  X-Content-Type-Options nosniff, and a restrictive Allow of GET, HEAD, OPTIONS.\n  No CAA records, no SPF record, and DMARC is present only at p=none; DNSSEC is\n  not enabled on abstractapi.com. Probed live 2026-07-12.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/abstractapi-phone/refs/heads/main/security/abstractapi-phone-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Number Verification
- Phone Validation
- Phone Number
- Phone Number Lookup
- Verification
- Carrier Lookup
- Line Type
- Data Validation
---
