---
api_specs:
- filename: customer-io-track-api-openapi.yml
  format: yaml
  label: Customer.io Track API
  slug: track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customer-io/refs/heads/main/openapi/customer-io-track-api-openapi.yml
- filename: customer-io-app-api-openapi.yml
  format: yaml
  label: Customer.io App API
  slug: app-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customer-io/refs/heads/main/openapi/customer-io-app-api-openapi.yml
- filename: customer-io-pipelines-api-openapi.yml
  format: yaml
  label: Customer.io Pipelines API
  slug: pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customer-io/refs/heads/main/openapi/customer-io-pipelines-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: customer.io
  spf: true
hosts:
- cert_expires: Sep 22 13:17:15 2026 GMT
  host: customer.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 26 05:13:46 2026 GMT
  host: docs.customer.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  4 02:31:30 2026 GMT
  host: track.customer.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Customer Io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Customer.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Customer.io
provider_slug: customer-io
slug: customer-io-domain-security
source_filename: customer-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: customer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:17:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.customer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 05:13:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: track.customer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:31:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: customer.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/customer-io/refs/heads/main/security/customer-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Behavioral Data
- Broadcasts
- Campaigns
- CDP
- Customer Data
- Customer Data Platform
- Data Ingestion
- Email
- Event Tracking
- Marketing Automation
- Messaging
- Push Notifications
- Segments
- SMS
- Transactional Email
---
