---
api_specs:
- filename: tech-data-authentication-api-openapi.yml
  format: yaml
  label: Tech Data Authentication API
  slug: tech-data-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-authentication-api-openapi.yml
- filename: tech-data-cart-items-api-openapi.yml
  format: yaml
  label: Tech Data Cart Items API
  slug: tech-data-cart-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-cart-items-api-openapi.yml
- filename: tech-data-carts-api-openapi.yml
  format: yaml
  label: Tech Data Carts API
  slug: tech-data-carts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-carts-api-openapi.yml
- filename: tech-data-cloud-providers-api-openapi.yml
  format: yaml
  label: Tech Data Cloud Providers API
  slug: tech-data-cloud-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-cloud-providers-api-openapi.yml
- filename: tech-data-customers-api-openapi.yml
  format: yaml
  label: Tech Data Customers API
  slug: tech-data-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-customers-api-openapi.yml
- filename: tech-data-orders-api-openapi.yml
  format: yaml
  label: Tech Data Orders API
  slug: tech-data-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-orders-api-openapi.yml
- filename: tech-data-products-api-openapi.yml
  format: yaml
  label: Tech Data Products API
  slug: tech-data-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-products-api-openapi.yml
- filename: tech-data-provisioning-templates-api-openapi.yml
  format: yaml
  label: Tech Data Provisioning Templates API
  slug: tech-data-provisioning-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-provisioning-templates-api-openapi.yml
- filename: tech-data-reports-api-openapi.yml
  format: yaml
  label: Tech Data Reports API
  slug: tech-data-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-reports-api-openapi.yml
- filename: tech-data-subscriptions-api-openapi.yml
  format: yaml
  label: Tech Data Subscriptions API
  slug: tech-data-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/openapi/tech-data-subscriptions-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: tdsynnex.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: streamone.cloud
  spf: true
hosts:
- cert_expires: Nov 11 11:31:17 2026 GMT
  host: www.tdsynnex.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 11:01:06 2026 GMT
  host: docs.streamone.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 19 16:53:40 2026 GMT
  host: ion.tdsynnex.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Tech Data Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tech Data, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Tech Data
provider_slug: tech-data
slug: tech-data-domain-security
source_filename: tech-data-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.tdsynnex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 11 11:31:17 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: docs.streamone.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 11:01:06 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: ion.tdsynnex.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 19 16:53:40 2026 GMT\n  hsts: null\ndomains:\n- domain: tdsynnex.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: streamone.cloud\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tech-data/refs/heads/main/security/tech-data-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cloud
- Distribution
- Information Technology
- Partner
- Fortune 500
---
