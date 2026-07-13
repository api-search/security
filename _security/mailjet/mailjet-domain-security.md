---
api_specs:
- filename: mailjet-email-api-openapi.yml
  format: yaml
  label: Mailjet Email API
  slug: mailjet-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-email-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: mailjet.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: dev.mailjet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.mailjet.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mailjet Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mailjet, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Mailjet
provider_slug: mailjet
slug: mailjet-domain-security
source_filename: mailjet-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dev.mailjet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\n- host: api.mailjet.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mailjet.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/security/mailjet-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Email
- Email Delivery
- Marketing Email
- SMTP
- Transactional Email
---
