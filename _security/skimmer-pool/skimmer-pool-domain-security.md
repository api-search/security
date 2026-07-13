---
api_specs:
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Customers API
  slug: skimmer-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Bodies of Water API
  slug: skimmer-bodies-of-water-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Service Locations API
  slug: skimmer-service-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Work Orders API
  slug: skimmer-work-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Routes API
  slug: skimmer-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Invoices and Billing API
  slug: skimmer-invoices-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Quotes API
  slug: skimmer-quotes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Products API
  slug: skimmer-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
- filename: skimmer-pool-openapi.yml
  format: yaml
  label: Skimmer Users API
  slug: skimmer-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/openapi/skimmer-pool-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: getskimmer.com
  spf: true
hosts:
- cert_expires: Aug 16 11:26:23 2026 GMT
  host: www.getskimmer.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  4 01:47:28 2026 GMT
  host: devportal.getskimmer.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 07:00:48 2026 GMT
  host: publicapi.getskimmer.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Skimmer Pool Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Skimmer, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Skimmer
provider_slug: skimmer-pool
slug: skimmer-pool-domain-security
source_filename: skimmer-pool-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.getskimmer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 16 11:26:23 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: devportal.getskimmer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  4 01:47:28 2026 GMT\n  hsts: false\n- host: publicapi.getskimmer.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 07:00:48 2026 GMT\n  hsts: null\ndomains:\n- domain: getskimmer.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skimmer-pool/refs/heads/main/security/skimmer-pool-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Pool Service
- Field Service Management
- Pool Maintenance
- Scheduling
- Routes
- Work Orders
- Invoicing
- Vertical SaaS
---
