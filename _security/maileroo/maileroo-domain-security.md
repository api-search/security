---
api_specs:
- filename: maileroo-email-api-openapi.yml
  format: yaml
  label: Maileroo Email API
  slug: maileroo-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/maileroo/refs/heads/main/openapi/maileroo-email-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: maileroo.com
  spf: true
hosts:
- cert_expires: Sep 15 21:02:48 2026 GMT
  host: maileroo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec  6 23:59:59 2026 GMT
  host: smtp.maileroo.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Maileroo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Maileroo, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Maileroo
provider_slug: maileroo
slug: maileroo-domain-security
source_filename: maileroo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: maileroo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 21:02:48 2026 GMT\n  hsts: false\n- host: smtp.maileroo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  6 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: maileroo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/maileroo/refs/heads/main/security/maileroo-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Email
- Email Delivery
- Marketing Email
- SMTP
- Transactional Email
---
