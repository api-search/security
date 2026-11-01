---
api_specs:
- filename: withreach-transaction-details-api-openapi.yml
  format: yaml
  label: Transaction Details API
  slug: transaction-details-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/withreach/openapi/withreach-transaction-details-api-openapi.yml
- filename: withreach-get-api-openapi.yml
  format: yaml
  label: Reach GET API
  slug: withreach-get-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/withreach/openapi/withreach-get-api-openapi.yml
- filename: withreach-order-api-openapi.yml
  format: yaml
  label: Reach Order API
  slug: withreach-order-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/withreach/openapi/withreach-order-api-openapi.yml
- filename: withreach-post-api-openapi.yml
  format: yaml
  label: Reach POST API
  slug: withreach-post-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/withreach/openapi/withreach-post-api-openapi.yml
- filename: withreach-quote-api-openapi.yml
  format: yaml
  label: Reach Quote API
  slug: withreach-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/withreach/openapi/withreach-quote-api-openapi.yml
- filename: withreach-session-api-openapi.yml
  format: yaml
  label: Reach Session API
  slug: withreach-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/withreach/openapi/withreach-session-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: withreach.com
  spf: true
hosts:
- cert_expires: Dec 23 22:37:15 2026 GMT
  host: www.withreach.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Withreach Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Reach, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Reach
provider_slug: withreach
slug: withreach-domain-security
source_filename: withreach-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.withreach.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 22:37:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: withreach.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/withreach/security/withreach-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Payments
- Tax
- Compliance
- E-commerce
- Merchant of Record
---
