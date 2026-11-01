---
api_specs:
- filename: answerline-dev-async-api-openapi.yml
  format: yaml
  label: answerline-dev Async API
  slug: answerline-dev-async-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/answerline-dev/openapi/answerline-dev-async-api-openapi.yml
- filename: answerline-dev-countries-api-openapi.yml
  format: yaml
  label: answerline-dev Countries API
  slug: answerline-dev-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/answerline-dev/openapi/answerline-dev-countries-api-openapi.yml
- filename: answerline-dev-credits-api-openapi.yml
  format: yaml
  label: answerline-dev Credits API
  slug: answerline-dev-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/answerline-dev/openapi/answerline-dev-credits-api-openapi.yml
- filename: answerline-dev-monitor-api-openapi.yml
  format: yaml
  label: answerline-dev Monitor API
  slug: answerline-dev-monitor-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/answerline-dev/openapi/answerline-dev-monitor-api-openapi.yml
- filename: answerline-dev-states-api-openapi.yml
  format: yaml
  label: answerline-dev States API
  slug: answerline-dev-states-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/answerline-dev/openapi/answerline-dev-states-api-openapi.yml
description: ''
domains:
- caa:
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog; cansignhttpexchanges=yes"
  - 0 issue "sectigo.com"
  - 0 issue "ssl.com"
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: answerline.dev
  spf: true
hosts:
- cert_expires: Dec 14 22:35:19 2026 GMT
  host: answerline.dev
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Answerline Dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for answerline-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: answerline-dev
provider_slug: answerline-dev
slug: answerline-dev-domain-security
source_filename: answerline-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: answerline.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 14 22:35:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: answerline.dev\n  dnssec: true\n  caa:\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"ssl.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/answerline-dev/security/answerline-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Visibility
- Marketing
- Analytics
- API
---
