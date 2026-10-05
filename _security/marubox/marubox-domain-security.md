---
api_specs:
- filename: marubox-account-api-openapi.yml
  format: yaml
  label: Business Box Account API
  slug: marubox-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-account-api-openapi.yml
- filename: marubox-bookings-api-openapi.yml
  format: yaml
  label: Business Box Bookings API
  slug: marubox-bookings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-bookings-api-openapi.yml
- filename: marubox-event-types-api-openapi.yml
  format: yaml
  label: Business Box Event types API
  slug: marubox-event-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-event-types-api-openapi.yml
- filename: marubox-invites-api-openapi.yml
  format: yaml
  label: Business Box Invites API
  slug: marubox-invites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-invites-api-openapi.yml
- filename: marubox-webhooks-api-openapi.yml
  format: yaml
  label: Business Box Webhooks API
  slug: marubox-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/openapi/marubox-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: marubox.jp
  spf: true
hosts:
- cert_expires: Dec 20 06:11:01 2026 GMT
  host: marubox.jp
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 19 00:13:23 2026 GMT
  host: api.marubox.jp
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Marubox Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Business Box, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Business Box
provider_slug: marubox
slug: marubox-domain-security
source_filename: marubox-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: marubox.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 06:11:01 2026 GMT\n  hsts: false\n- host: api.marubox.jp\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 00:13:23 2026 GMT\n  hsts: null\ndomains:\n- domain: marubox.jp\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/marubox/refs/heads/main/security/marubox-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Booking
- Payments
- Calendar
- Japan
---
