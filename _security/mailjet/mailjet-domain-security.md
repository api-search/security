---
api_specs:
- filename: mailjet-campaigns-api-openapi.yml
  format: yaml
  label: Mailjet Campaigns API
  slug: mailjet-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-campaigns-api-openapi.yml
- filename: mailjet-contact-lists-api-openapi.yml
  format: yaml
  label: Mailjet Contact Lists API
  slug: mailjet-contact-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-contact-lists-api-openapi.yml
- filename: mailjet-contacts-api-openapi.yml
  format: yaml
  label: Mailjet Contacts API
  slug: mailjet-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-contacts-api-openapi.yml
- filename: mailjet-event-api-openapi.yml
  format: yaml
  label: Mailjet Event API
  slug: mailjet-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-event-api-openapi.yml
- filename: mailjet-send-api-openapi.yml
  format: yaml
  label: Mailjet Send API
  slug: mailjet-send-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-send-api-openapi.yml
- filename: mailjet-senders-api-openapi.yml
  format: yaml
  label: Mailjet Senders API
  slug: mailjet-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-senders-api-openapi.yml
- filename: mailjet-statistics-api-openapi.yml
  format: yaml
  label: Mailjet Statistics API
  slug: mailjet-statistics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-statistics-api-openapi.yml
- filename: mailjet-templates-api-openapi.yml
  format: yaml
  label: Mailjet Templates API
  slug: mailjet-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mailjet/refs/heads/main/openapi/mailjet-templates-api-openapi.yml
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
