---
api_specs:
- filename: honeybadger-webhooks-asyncapi.yml
  format: yaml
  label: Honeybadger Outbound Webhook Notifications
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybadger/refs/heads/main/asyncapi/honeybadger-webhooks-asyncapi.yml
description: ''
domains:
- caa:
  - 0 issuewild "awstrust.com"
  - 0 issuewild "sectigo.com"
  - 0 issue "amazon.com"
  - 0 issue "amazonaws.com"
  - 0 issue "amazontrust.com"
  - 0 issue "awstrust.com"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: honeybadger.io
  spf: true
hosts:
- cert_expires: Aug 25 21:13:53 2026 GMT
  host: www.honeybadger.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 10:43:41 2026 GMT
  host: docs.honeybadger.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 28 23:59:59 2026 GMT
  host: api.honeybadger.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Honeybadger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Honeybadger, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Honeybadger
provider_slug: honeybadger
slug: honeybadger-domain-security
source_filename: honeybadger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.honeybadger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 25 21:13:53 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.honeybadger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 10:43:41 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.honeybadger.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 28 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: honeybadger.io\n  dnssec: false\n  caa:\n  - 0 issuewild \"awstrust.com\"\n  - 0 issuewild \"sectigo.com\"\n  - 0 issue \"amazon.com\"\n  - 0 issue \"amazonaws.com\"\n  - 0 issue \"amazontrust.com\"\n  - 0 issue \"awstrust.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honeybadger/refs/heads/main/security/honeybadger-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Error Monitoring
- Exception Tracking
- Application Performance Monitoring
- Uptime Monitoring
- Cron Monitoring
- Observability
---
