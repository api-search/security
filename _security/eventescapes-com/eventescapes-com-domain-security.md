---
api_specs:
- filename: eventescapes-com-events-api-openapi.yml
  format: yaml
  label: Event Escapes Events API
  slug: eventescapes-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventescapes-com/openapi/eventescapes-com-events-api-openapi.yml
- filename: eventescapes-com-experiences-api-openapi.yml
  format: yaml
  label: Event Escapes Experiences API
  slug: eventescapes-com-experiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventescapes-com/openapi/eventescapes-com-experiences-api-openapi.yml
- filename: eventescapes-com-packages-api-openapi.yml
  format: yaml
  label: Event Escapes Packages API
  slug: eventescapes-com-packages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventescapes-com/openapi/eventescapes-com-packages-api-openapi.yml
- filename: eventescapes-com-payment-links-api-openapi.yml
  format: yaml
  label: Event Escapes Payment Links API
  slug: eventescapes-com-payment-links-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventescapes-com/openapi/eventescapes-com-payment-links-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "ssl.com"
  - 0 issuewild "comodoca.com"
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eventescapes.com
  spf: true
hosts:
- cert_expires: Dec 10 08:16:58 2026 GMT
  host: eventescapes.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Event Escapes Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Event Escapes, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Event Escapes
provider_slug: eventescapes-com
slug: eventescapes-com-domain-security
source_filename: eventescapes-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eventescapes.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 10 08:16:58 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eventescapes.com\n  dnssec: false\n  caa:\n  - 0 issue \"ssl.com\"\n  - 0 issuewild \"comodoca.com\"\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/eventescapes-com/security/eventescapes-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Travel
- Event
- Ticketing
- Hotels
- Sports
---
