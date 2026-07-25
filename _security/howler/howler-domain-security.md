---
api_specs:
- filename: howler-artists-api-openapi.yml
  format: yaml
  label: Howler Artists API
  slug: howler-artists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-artists-api-openapi.yml
- filename: howler-assign-ticket-api-openapi.yml
  format: yaml
  label: Howler Assign Ticket API
  slug: howler-assign-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-assign-ticket-api-openapi.yml
- filename: howler-bank-account-api-openapi.yml
  format: yaml
  label: Howler Bank Account API
  slug: howler-bank-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-bank-account-api-openapi.yml
- filename: howler-basic-authentication-api-openapi.yml
  format: yaml
  label: Howler Basic Authentication API
  slug: howler-basic-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-basic-authentication-api-openapi.yml
- filename: howler-cashless-tags-api-openapi.yml
  format: yaml
  label: Howler Cashless Tags API
  slug: howler-cashless-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-cashless-tags-api-openapi.yml
- filename: howler-cashout-api-openapi.yml
  format: yaml
  label: Howler Cashout API
  slug: howler-cashout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-cashout-api-openapi.yml
- filename: howler-email-otp-api-openapi.yml
  format: yaml
  label: Howler Email OTP API
  slug: howler-email-otp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-email-otp-api-openapi.yml
- filename: howler-events-api-openapi.yml
  format: yaml
  label: Howler Events API
  slug: howler-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-events-api-openapi.yml
- filename: howler-oauth-api-openapi.yml
  format: yaml
  label: Howler OAuth API
  slug: howler-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-oauth-api-openapi.yml
- filename: howler-third-party-oauth-api-openapi.yml
  format: yaml
  label: Howler Third Party OAuth API
  slug: howler-third-party-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-third-party-oauth-api-openapi.yml
- filename: howler-tickets-api-openapi.yml
  format: yaml
  label: Howler Tickets API
  slug: howler-tickets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-tickets-api-openapi.yml
- filename: howler-top-up-api-openapi.yml
  format: yaml
  label: Howler Top Up API
  slug: howler-top-up-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-top-up-api-openapi.yml
- filename: howler-top-up-cashless-tag-api-openapi.yml
  format: yaml
  label: Howler Top Up Cashless Tag API
  slug: howler-top-up-cashless-tag-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-top-up-cashless-tag-api-openapi.yml
- filename: howler-top-up-ticket-api-openapi.yml
  format: yaml
  label: Howler Top Up Ticket API
  slug: howler-top-up-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-top-up-ticket-api-openapi.yml
- filename: howler-topupables-api-openapi.yml
  format: yaml
  label: Howler Topupables API
  slug: howler-topupables-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-topupables-api-openapi.yml
- filename: howler-transfer-ticket-api-openapi.yml
  format: yaml
  label: Howler Transfer Ticket API
  slug: howler-transfer-ticket-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-transfer-ticket-api-openapi.yml
- filename: howler-user-api-openapi.yml
  format: yaml
  label: Howler User API
  slug: howler-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/openapi/howler-user-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: howler.co.za
  spf: true
hosts:
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: howler.co.za
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Howler Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Howler, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Howler
provider_slug: howler
slug: howler-domain-security
source_filename: howler-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: howler.co.za\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: howler.co.za\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/howler/refs/heads/main/security/howler-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Events
- Ticketing
- Payments
- Cashless
- RFID
- Event Management
- Fintech
- South Africa
---
