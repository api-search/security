---
api_specs:
- filename: onesignal-openapi.yml
  format: yaml
  label: OneSignal Messages API
  slug: onesignal-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onesignal/refs/heads/main/openapi/onesignal-openapi.yml
- filename: onesignal-openapi.yml
  format: yaml
  label: OneSignal Users & Subscriptions API
  slug: onesignal-users-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onesignal/refs/heads/main/openapi/onesignal-openapi.yml
- filename: onesignal-openapi.yml
  format: yaml
  label: OneSignal Segments API
  slug: onesignal-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onesignal/refs/heads/main/openapi/onesignal-openapi.yml
- filename: onesignal-openapi.yml
  format: yaml
  label: OneSignal Apps & Keys API
  slug: onesignal-apps-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onesignal/refs/heads/main/openapi/onesignal-openapi.yml
- filename: onesignal-openapi.yml
  format: yaml
  label: OneSignal Exports & Analytics API
  slug: onesignal-exports-analytics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/onesignal/refs/heads/main/openapi/onesignal-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: onesignal.com
  spf: true
hosts:
- cert_expires: Sep 11 17:06:32 2026 GMT
  host: onesignal.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 17:59:01 2026 GMT
  host: documentation.onesignal.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 11 15:32:24 2026 GMT
  host: api.onesignal.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Onesignal Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OneSignal, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: OneSignal
provider_slug: onesignal
slug: onesignal-domain-security
source_filename: onesignal-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: onesignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 17:06:32 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: documentation.onesignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 17:59:01 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.onesignal.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 11 15:32:24 2026 GMT\n  hsts: null\ndomains:\n- domain: onesignal.com\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/onesignal/refs/heads/main/security/onesignal-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Notifications
- Push
- Email
- SMS
- Mobile
---
