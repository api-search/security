---
api_specs:
- filename: tito-openapi.yml
  format: yaml
  label: Tito Events API
  slug: tito-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Releases API
  slug: tito-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Tickets API
  slug: tito-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Registrations API
  slug: tito-registrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Discount Codes API
  slug: tito-discount-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Activities API
  slug: tito-activities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Check-in Lists API
  slug: tito-check-in-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Refunds API
  slug: tito-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
- filename: tito-openapi.yml
  format: yaml
  label: Tito Webhook Endpoints API
  slug: tito-webhook-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/openapi/tito-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: tito.io
  spf: true
  spf_record: v=spf1 a include:_spf.google.com include:spf.mail.intercom.io include:helpscoutemail.com include:amazonses.com ~all
hosts:
- cert_expires: Aug 19 10:53:44 2026 GMT
  host: tito.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 10:53:44 2026 GMT
  host: ti.to
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  1 07:41:56 2026 GMT
  host: api.tito.io
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tito Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tito, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Tito
provider_slug: tito
slug: tito-domain-security
source_filename: tito-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tito.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 10:53:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: ti.to\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 10:53:44 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\n- host: api.tito.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  1 07:41:56 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n  hsts_include_subdomains: true\ndomains:\n- domain: tito.io\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 a include:_spf.google.com include:spf.mail.intercom.io include:helpscoutemail.com include:amazonses.com ~all\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tito/refs/heads/main/security/tito-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Event Ticketing
- Events
- Registration
- Ticketing
- Conferences
- Event Management
- Attendees
- Webhooks
- SaaS
---
