---
api_specs:
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Reservations API
  slug: smoobu-reservations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Apartments API
  slug: smoobu-apartments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Rates and Availability API
  slug: smoobu-rates-availability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Guests API
  slug: smoobu-guests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Messaging API
  slug: smoobu-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
- filename: smoobu-openapi.yml
  format: yaml
  label: Smoobu Webhooks
  slug: smoobu-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/openapi/smoobu-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: smoobu.com
  spf: true
hosts:
- cert_expires: Aug 19 19:29:12 2026 GMT
  host: www.smoobu.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 19:29:12 2026 GMT
  host: docs.smoobu.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 19:29:12 2026 GMT
  host: login.smoobu.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Smoobu Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Smoobu, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Smoobu
provider_slug: smoobu
slug: smoobu-domain-security
source_filename: smoobu-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.smoobu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 19:29:12 2026 GMT\n  hsts: false\n- host: docs.smoobu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 19:29:12 2026 GMT\n  hsts: false\n- host: login.smoobu.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 19:29:12 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: smoobu.com\n  dnssec: true\n  caa:\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smoobu/refs/heads/main/security/smoobu-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Vacation Rental
- Channel Manager
- Property Management
- Short-Term Rental
- Reservations
- Hospitality
---
