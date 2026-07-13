---
api_specs:
- filename: qstash-api-openapi.yml
  format: yaml
  label: QStash API
  slug: qstash-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/qstash/refs/heads/main/openapi/qstash-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: upstash.com
  spf: true
- caa:
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  dmarc: false
  dnssec: false
  domain: upstash.io
  spf: false
hosts:
- cert_expires: Aug 21 18:18:03 2026 GMT
  host: upstash.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 31 23:59:59 2026 GMT
  host: qstash.upstash.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Qstash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for QStash, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: QStash
provider_slug: qstash
slug: qstash-domain-security
source_filename: qstash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: upstash.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 18:18:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: qstash.upstash.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 31 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: upstash.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: upstash.io\n  dnssec: false\n  caa:\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/qstash/refs/heads/main/security/qstash-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Message Queue
- Task Scheduling
- Serverless
- HTTP Messaging
- Background Jobs
- Webhooks
- Dead Letter Queue
- CRON
- Upstash
---
