---
api_specs:
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Shops API
  slug: tekmetric-shops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Customers API
  slug: tekmetric-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Vehicles API
  slug: tekmetric-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Repair Orders API
  slug: tekmetric-repair-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Jobs API
  slug: tekmetric-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Employees API
  slug: tekmetric-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Appointments API
  slug: tekmetric-appointments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Inventory API
  slug: tekmetric-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
- filename: tekmetric-openapi.yml
  format: yaml
  label: Tekmetric Canned Jobs API
  slug: tekmetric-canned-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/openapi/tekmetric-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tekmetric.com
  spf: true
hosts:
- cert_expires: Oct  9 03:07:19 2026 GMT
  host: www.tekmetric.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: api.tekmetric.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 23:59:59 2026 GMT
  host: shop.tekmetric.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tekmetric Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tekmetric, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tekmetric
provider_slug: tekmetric
slug: tekmetric-domain-security
source_filename: tekmetric-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tekmetric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  9 03:07:19 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tekmetric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: shop.tekmetric.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: tekmetric.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tekmetric/refs/heads/main/security/tekmetric-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Automotive
- Auto Repair
- Shop Management
- Fleet
- Vertical SaaS
---
