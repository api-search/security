---
api_specs:
- filename: resend-openapi.yml
  format: yaml
  label: Resend API
  slug: resend
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/openapi/resend-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: resend.com
  spf: true
hosts:
- cert_expires: Sep 28 17:52:04 2026 GMT
  host: resend.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 12 13:48:19 2026 GMT
  host: api.resend.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Resend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Resend, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Resend
provider_slug: resend
slug: resend-domain-security
source_filename: resend-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: resend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 17:52:04 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.resend.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 13:48:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: resend.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/resend/refs/heads/main/security/resend-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Developer Tools
- Transactional Email
- Marketing Email
---
