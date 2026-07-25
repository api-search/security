---
api_specs:
- filename: customerio-broadcasts-api-openapi.yml
  format: yaml
  label: Customer.io Broadcasts API
  slug: customerio-broadcasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-broadcasts-api-openapi.yml
- filename: customerio-campaigns-api-openapi.yml
  format: yaml
  label: Customer.io Campaigns API
  slug: customerio-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-campaigns-api-openapi.yml
- filename: customerio-collections-api-openapi.yml
  format: yaml
  label: Customer.io Collections API
  slug: customerio-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-collections-api-openapi.yml
- filename: customerio-customers-api-openapi.yml
  format: yaml
  label: Customer.io Customers API
  slug: customerio-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-customers-api-openapi.yml
- filename: customerio-devices-api-openapi.yml
  format: yaml
  label: Customer.io Devices API
  slug: customerio-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-devices-api-openapi.yml
- filename: customerio-events-api-openapi.yml
  format: yaml
  label: Customer.io Events API
  slug: customerio-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-events-api-openapi.yml
- filename: customerio-exports-api-openapi.yml
  format: yaml
  label: Customer.io Exports API
  slug: customerio-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-exports-api-openapi.yml
- filename: customerio-messages-api-openapi.yml
  format: yaml
  label: Customer.io Messages API
  slug: customerio-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-messages-api-openapi.yml
- filename: customerio-people-api-openapi.yml
  format: yaml
  label: Customer.io People API
  slug: customerio-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-people-api-openapi.yml
- filename: customerio-pipelines-api-openapi.yml
  format: yaml
  label: Customer.io Pipelines API
  slug: customerio-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-pipelines-api-openapi.yml
- filename: customerio-segments-api-openapi.yml
  format: yaml
  label: Customer.io Segments API
  slug: customerio-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-segments-api-openapi.yml
- filename: customerio-track-v2-api-openapi.yml
  format: yaml
  label: Customer.io Track v2 API
  slug: customerio-track-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-track-v2-api-openapi.yml
- filename: customerio-transactional-api-openapi.yml
  format: yaml
  label: Customer.io Transactional API
  slug: customerio-transactional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/openapi/customerio-transactional-api-openapi.yml
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
name: Customerio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Customer.io, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Customer.io
provider_slug: customerio
slug: customerio-domain-security
source_filename: customerio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: customer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 13:17:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.customer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 26 05:13:46 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: track.customer.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  4 02:31:30 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: customer.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/customerio/refs/heads/main/security/customerio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Customer Messaging
- Marketing Automation
- Email
- CDP
- Transactional
---
