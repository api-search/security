---
api_specs:
- filename: mailtrap-email-api-openapi.yml
  format: yaml
  label: Mailtrap Email Sending API
  slug: mailtrap-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailtrap/refs/heads/main/openapi/mailtrap-email-api-openapi.yml
- filename: mailtrap-email-sandbox-openapi.yml
  format: yaml
  label: Mailtrap Email Sandbox API
  slug: mailtrap-email-sandbox
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailtrap/refs/heads/main/openapi/mailtrap-email-sandbox-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailtrap.io
  spf: true
hosts:
- cert_expires: Aug 12 17:17:20 2026 GMT
  host: mailtrap.io
  hsts: true
  hsts_max_age: 0
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 04:53:53 2026 GMT
  host: send.api.mailtrap.io
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 12 04:53:53 2026 GMT
  host: sandbox.api.mailtrap.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mailtrap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailtrap, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mailtrap
provider_slug: mailtrap
slug: mailtrap-domain-security
source_filename: mailtrap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailtrap.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 12 17:17:20 2026 GMT\n  hsts: true\n  hsts_max_age: 0\n- host: send.api.mailtrap.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:53:53 2026 GMT\n  hsts: null\n- host: sandbox.api.mailtrap.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 04:53:53 2026 GMT\n  hsts: null\ndomains:\n- domain: mailtrap.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailtrap/refs/heads/main/security/mailtrap-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Email Delivery
- Email Sandbox
- Email Testing
- Transactional Email
---
