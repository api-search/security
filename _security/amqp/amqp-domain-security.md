---
api_specs:
- filename: amqp-messaging.yml
  format: yaml
  label: AMQP Messaging API
  slug: amqp-messaging-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/amqp/refs/heads/main/asyncapi/amqp-messaging.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: amqp.org
  spf: false
hosts:
- cert_expires: Sep  3 18:15:37 2026 GMT
  host: www.amqp.org
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amqp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for AMQP, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: AMQP
provider_slug: amqp
slug: amqp-domain-security
source_filename: amqp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amqp.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 18:15:37 2026 GMT\n  hsts: false\ndomains:\n- domain: amqp.org\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amqp/refs/heads/main/security/amqp-domain-security.yml
summary_line: TLSv1.3
tags:
- AMQP
- Asynchronous
- Message Queue
- Messaging
- Middleware
- Open Standard
- Publish Subscribe
---
