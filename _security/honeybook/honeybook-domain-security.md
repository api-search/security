---
api_specs:
- filename: honeybook-clients-api-openapi.yml
  format: yaml
  label: HoneyBook Clients API
  slug: honeybook-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-clients-api-openapi.yml
- filename: honeybook-contracts-api-openapi.yml
  format: yaml
  label: HoneyBook Contracts API
  slug: honeybook-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-contracts-api-openapi.yml
- filename: honeybook-invoices-api-openapi.yml
  format: yaml
  label: HoneyBook Invoices API
  slug: honeybook-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-invoices-api-openapi.yml
- filename: honeybook-payments-api-openapi.yml
  format: yaml
  label: HoneyBook Payments API
  slug: honeybook-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-payments-api-openapi.yml
- filename: honeybook-projects-api-openapi.yml
  format: yaml
  label: HoneyBook Projects API
  slug: honeybook-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-projects-api-openapi.yml
- filename: honeybook-proposals-api-openapi.yml
  format: yaml
  label: HoneyBook Proposals API
  slug: honeybook-proposals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-proposals-api-openapi.yml
- filename: honeybook-scheduler-api-openapi.yml
  format: yaml
  label: HoneyBook Scheduler API
  slug: honeybook-scheduler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-scheduler-api-openapi.yml
- filename: honeybook-webhooks-api-openapi.yml
  format: yaml
  label: HoneyBook Webhooks API
  slug: honeybook-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/openapi/honeybook-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: honeybook.com
  spf: true
hosts:
- cert_expires: Nov 12 16:33:10 2026 GMT
  host: www.honeybook.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 17 07:12:24 2026 GMT
  host: help.honeybook.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 20 03:36:07 2026 GMT
  host: api.honeybook.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: Honeybook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HoneyBook, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: HoneyBook
provider_slug: honeybook
slug: honeybook-domain-security
source_filename: honeybook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.honeybook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 12 16:33:10 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: help.honeybook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 07:12:24 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: api.honeybook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 20 03:36:07 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: honeybook.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honeybook/refs/heads/main/security/honeybook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- CRM
- Clientflow
- Proposals
- Contracts
- Invoicing
- Payments
- Scheduling
- Creative Entrepreneurs
- Small Business
---
