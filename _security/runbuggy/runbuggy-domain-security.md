---
api_specs:
- filename: runbuggy-companies-api-openapi.yml
  format: yaml
  label: RunBuggy Companies API
  slug: runbuggy-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-companies-api-openapi.yml
- filename: runbuggy-orders-api-openapi.yml
  format: yaml
  label: RunBuggy Orders API
  slug: runbuggy-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-orders-api-openapi.yml
- filename: runbuggy-token-api-openapi.yml
  format: yaml
  label: RunBuggy Token API
  slug: runbuggy-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-token-api-openapi.yml
- filename: runbuggy-vehicle-transfer-orders-api-openapi.yml
  format: yaml
  label: RunBuggy Vehicle Transfer Orders API
  slug: runbuggy-vehicle-transfer-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-vehicle-transfer-orders-api-openapi.yml
- filename: runbuggy-webhooks-api-openapi.yml
  format: yaml
  label: RunBuggy Webhooks API
  slug: runbuggy-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/openapi/runbuggy-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: runbuggy.com
  spf: true
hosts:
- cert_expires: Sep 22 23:52:48 2026 GMT
  host: runbuggy.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 11:29:00 2026 GMT
  host: docs.runbuggy.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 15 23:59:59 2026 GMT
  host: ng-staging.runbuggy.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Runbuggy Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for RunBuggy, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: RunBuggy
provider_slug: runbuggy
slug: runbuggy-domain-security
source_filename: runbuggy-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: runbuggy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 22 23:52:48 2026 GMT\n  hsts: false\n- host: docs.runbuggy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 11:29:00 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ng-staging.runbuggy.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 15 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: runbuggy.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/runbuggy/refs/heads/main/security/runbuggy-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Automotive
- Logistics
- Transportation
- Vehicle Shipping
- Marketplace
- Supply Chain
- Fleet
- TMS
- Freight
---
