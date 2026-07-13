---
api_specs:
- filename: mailgun.yaml
  format: yaml
  label: Mailgun Send API
  slug: send-api
  spec_type: OpenAPI
  url: https://documentation.mailgun.com/_spec/docs/mailgun/api-reference/send/mailgun.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailgun.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailgun.net
  spf: true
hosts:
- cert_expires: Aug 25 07:03:07 2026 GMT
  host: www.mailgun.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  9 13:38:27 2026 GMT
  host: documentation.mailgun.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  8 23:59:59 2026 GMT
  host: api.mailgun.net
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Mailgun Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailgun, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mailgun
provider_slug: mailgun
slug: mailgun-domain-security
source_filename: mailgun-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.mailgun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 07:03:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: documentation.mailgun.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 13:38:27 2026 GMT\n  hsts: false\n- host: api.mailgun.net\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Sep  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mailgun.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: mailgun.net\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailgun/refs/heads/main/security/mailgun-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Transactional Email
- SMTP
- Email Validation
- Email Delivery
- Messaging
---
