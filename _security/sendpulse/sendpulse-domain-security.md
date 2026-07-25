---
api_specs:
- filename: sendpulse-account-api-openapi.yml
  format: yaml
  label: SendPulse Account API
  slug: sendpulse-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-account-api-openapi.yml
- filename: sendpulse-address-books-api-openapi.yml
  format: yaml
  label: SendPulse Address Books API
  slug: sendpulse-address-books-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-address-books-api-openapi.yml
- filename: sendpulse-authorization-api-openapi.yml
  format: yaml
  label: SendPulse Authorization API
  slug: sendpulse-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-authorization-api-openapi.yml
- filename: sendpulse-automation-360-api-openapi.yml
  format: yaml
  label: SendPulse Automation 360 API
  slug: sendpulse-automation-360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-automation-360-api-openapi.yml
- filename: sendpulse-email-blacklist-api-openapi.yml
  format: yaml
  label: SendPulse Email Blacklist API
  slug: sendpulse-email-blacklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-email-blacklist-api-openapi.yml
- filename: sendpulse-email-campaigns-api-openapi.yml
  format: yaml
  label: SendPulse Email Campaigns API
  slug: sendpulse-email-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-email-campaigns-api-openapi.yml
- filename: sendpulse-senders-api-openapi.yml
  format: yaml
  label: SendPulse Senders API
  slug: sendpulse-senders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-senders-api-openapi.yml
- filename: sendpulse-sms-api-openapi.yml
  format: yaml
  label: SendPulse SMS API
  slug: sendpulse-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-sms-api-openapi.yml
- filename: sendpulse-smtp-api-openapi.yml
  format: yaml
  label: SendPulse SMTP API
  slug: sendpulse-smtp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-smtp-api-openapi.yml
- filename: sendpulse-web-push-api-openapi.yml
  format: yaml
  label: SendPulse Web Push API
  slug: sendpulse-web-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/openapi/sendpulse-web-push-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: sendpulse.com
  spf: true
hosts:
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: sendpulse.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Oct 29 23:59:59 2026 GMT
  host: api.sendpulse.com
  hsts: false
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Sendpulse Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for SendPulse, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.2); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: SendPulse
provider_slug: sendpulse
slug: sendpulse-domain-security
source_filename: sendpulse-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: sendpulse.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.sendpulse.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct 29 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: sendpulse.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sendpulse/refs/heads/main/security/sendpulse-domain-security.yml
summary_line: TLSv1.2 · HSTS · DMARC
tags:
- Marketing
- Email
- SMS
- Web Push
- Chatbots
- Transactional Email
- Multichannel
---
