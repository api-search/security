---
api_specs:
- filename: openapi.yml
  format: yaml
  label: GOV.UK Notify Notifications API
  slug: notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gov-uk-notify/refs/heads/main/openapi/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: service.gov.uk
  spf: true
hosts:
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: www.notifications.service.gov.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: docs.notifications.service.gov.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
- cert_expires: Jan 24 23:59:59 2027 GMT
  host: api.notifications.service.gov.uk
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gov Uk Notify Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for GOV.UK Notify, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: GOV.UK Notify
provider_slug: gov-uk-notify
slug: gov-uk-notify-domain-security
source_filename: gov-uk-notify-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.notifications.service.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.notifications.service.gov.uk\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.notifications.service.gov.uk\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 24 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: service.gov.uk\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gov-uk-notify/refs/heads/main/security/gov-uk-notify-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Notifications
- Email
- SMS
- Text Messages
- Letters
- Government
- United Kingdom
- Public Sector
- GDS
- REST
---
