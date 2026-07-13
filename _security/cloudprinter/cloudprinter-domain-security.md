---
api_specs:
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Orders API
  slug: cloudprinter-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Products & Pricing API
  slug: cloudprinter-products-pricing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Quotes API
  slug: cloudprinter-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Signal Webhooks API
  slug: cloudprinter-signal-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
- filename: cloudprinter-openapi.yml
  format: yaml
  label: Cloudprinter Files API
  slug: cloudprinter-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/openapi/cloudprinter-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: cloudprinter.com
  spf: true
hosts:
- cert_expires: Mar  1 23:59:59 2027 GMT
  host: www.cloudprinter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 13 23:59:59 2027 GMT
  host: docs.cloudprinter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 26 23:59:59 2026 GMT
  host: api.cloudprinter.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Cloudprinter Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cloudprinter, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Cloudprinter
provider_slug: cloudprinter
slug: cloudprinter-domain-security
source_filename: cloudprinter-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.cloudprinter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Mar  1 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.cloudprinter.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 23:59:59 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.cloudprinter.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Nov 26 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cloudprinter.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudprinter/refs/heads/main/security/cloudprinter-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Print on Demand
- Print Fulfillment
- Printing
- Orders
- Logistics
---
