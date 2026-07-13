---
api_specs:
- filename: cloudevents-http-asyncapi.yml
  format: yaml
  label: CloudEvents Specification
  slug: cloudevents-spec
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudevents/refs/heads/main/asyncapi/cloudevents-http-asyncapi.yml
- filename: cloudevents-subscriptions-openapi.yml
  format: yaml
  label: CloudEvents Subscriptions API
  slug: cloudevents-subscriptions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudevents/refs/heads/main/openapi/cloudevents-subscriptions-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: cloudevents.io
  spf: false
hosts:
- cert_expires: Oct  3 01:48:35 2026 GMT
  host: cloudevents.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Cloudevents Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CloudEvents, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: CloudEvents
provider_slug: cloudevents
slug: cloudevents-domain-security
source_filename: cloudevents-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cloudevents.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 01:48:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudevents.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudevents/refs/heads/main/security/cloudevents-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Cloud Native
- Events
- Graduated
- Interoperability
- Messaging
- Specification
---
