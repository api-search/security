---
api_specs:
- filename: eventsend-io-openapi-generated.yml
  format: yaml
  label: EventSend API
  slug: eventsend-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/eventsend-io/openapi/_ae-authored/eventsend-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: eventsend.io
  spf: true
hosts:
- cert_expires: Feb  3 06:32:28 2027 GMT
  host: eventsend.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: EventSend Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EventSend, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: EventSend
provider_slug: eventsend-io
slug: eventsend-io-domain-security
source_filename: eventsend-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: eventsend.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  3 06:32:28 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: eventsend.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/eventsend-io/security/eventsend-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Event Tracking
- Analytics
- Webhook
- Integration
- Product Teams
---
