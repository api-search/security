---
api_specs:
- filename: handlediq-com-booking-status-api-openapi.yml
  format: yaml
  label: handlediq-com Booking Status API
  slug: handlediq-com-booking-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-booking-status-api-openapi.yml
- filename: handlediq-com-cancel-booking-api-openapi.yml
  format: yaml
  label: handlediq-com Cancel Booking API
  slug: handlediq-com-cancel-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-cancel-booking-api-openapi.yml
- filename: handlediq-com-find-help-api-openapi.yml
  format: yaml
  label: handlediq-com Find Help API
  slug: handlediq-com-find-help-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-find-help-api-openapi.yml
- filename: handlediq-com-get-quote-api-openapi.yml
  format: yaml
  label: handlediq-com Get Quote API
  slug: handlediq-com-get-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-get-quote-api-openapi.yml
- filename: handlediq-com-hold-time-api-openapi.yml
  format: yaml
  label: handlediq-com Hold Time API
  slug: handlediq-com-hold-time-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-hold-time-api-openapi.yml
- filename: handlediq-com-move-booking-api-openapi.yml
  format: yaml
  label: handlediq-com Move Booking API
  slug: handlediq-com-move-booking-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-move-booking-api-openapi.yml
- filename: handlediq-com-request-service-api-openapi.yml
  format: yaml
  label: handlediq-com Request Service API
  slug: handlediq-com-request-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-request-service-api-openapi.yml
- filename: handlediq-com-verify-record-api-openapi.yml
  format: yaml
  label: handlediq-com Verify Record API
  slug: handlediq-com-verify-record-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/handlediq-com/openapi/handlediq-com-verify-record-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 iodef "mailto:mitch@handlediq.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: handlediq.com
  spf: true
hosts:
- cert_expires: Jan 21 17:51:57 2027 GMT
  host: handlediq.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Handlediq Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for handlediq-com, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: handlediq-com
provider_slug: handlediq-com
slug: handlediq-com-domain-security
source_filename: handlediq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: handlediq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 21 17:51:57 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: handlediq.com\n  dnssec: true\n  caa:\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 iodef \"mailto:mitch@handlediq.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/handlediq-com/security/handlediq-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Field Service
- SaaS
- Home Services
- Scheduling
- Payments
- AI
---
