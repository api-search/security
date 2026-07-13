---
api_specs:
- filename: mailpace-openapi.yml
  format: yaml
  label: MailPace Send Email API
  slug: mailpace-send-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailpace/refs/heads/main/openapi/mailpace-openapi.yml
- filename: mailpace-openapi.yml
  format: yaml
  label: MailPace Domains API
  slug: mailpace-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailpace/refs/heads/main/openapi/mailpace-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mailpace.com
  spf: true
hosts:
- cert_expires: Oct  7 02:13:47 2026 GMT
  host: mailpace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 27 02:03:39 2026 GMT
  host: docs.mailpace.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 20:58:38 2026 GMT
  host: app.mailpace.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mailpace Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MailPace, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: MailPace
provider_slug: mailpace
slug: mailpace-domain-security
source_filename: mailpace-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mailpace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 02:13:47 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.mailpace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 27 02:03:39 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: app.mailpace.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 20:58:38 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: mailpace.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailpace/refs/heads/main/security/mailpace-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Email
- Transactional Email
- Messaging
- SMTP
- Privacy
---
