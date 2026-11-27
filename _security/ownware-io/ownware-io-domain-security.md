---
api_specs:
- filename: ownware-io-customers-api-openapi.yml
  format: yaml
  label: Ownware Customers API
  slug: ownware-io-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ownware-io/openapi/ownware-io-customers-api-openapi.yml
- filename: ownware-io-licenses-api-openapi.yml
  format: yaml
  label: Ownware Licenses API
  slug: ownware-io-licenses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ownware-io/openapi/ownware-io-licenses-api-openapi.yml
- filename: ownware-io-orders-api-openapi.yml
  format: yaml
  label: Ownware Orders API
  slug: ownware-io-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ownware-io/openapi/ownware-io-orders-api-openapi.yml
- filename: ownware-io-ping-api-openapi.yml
  format: yaml
  label: Ownware Ping API
  slug: ownware-io-ping-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ownware-io/openapi/ownware-io-ping-api-openapi.yml
- filename: ownware-io-redeem-codes-api-openapi.yml
  format: yaml
  label: Ownware Redeem Codes API
  slug: ownware-io-redeem-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ownware-io/openapi/ownware-io-redeem-codes-api-openapi.yml
- filename: ownware-io-stats-api-openapi.yml
  format: yaml
  label: Ownware Stats API
  slug: ownware-io-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ownware-io/openapi/ownware-io-stats-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: ownware.io
  spf: true
hosts:
- cert_expires: Jan 27 06:13:33 2027 GMT
  host: ownware.io
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Ownware Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ownware, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Ownware
provider_slug: ownware-io
slug: ownware-io-domain-security
source_filename: ownware-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: ownware.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 27 06:13:33 2027 GMT\n  hsts: true\n  hsts_max_age: 15552000\ndomains:\n- domain: ownware.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/ownware-io/security/ownware-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Self‑Hosted Software
- Invoicing
- Appointment Booking
- Point-of-Sale
- Compliance Tools
- Expense Management
---
