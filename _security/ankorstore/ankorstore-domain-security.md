---
api_specs:
- filename: ankorstore-main-openapi-original.yml
  format: yaml
  label: Ankorstore Public API
  slug: ankorstore-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankorstore/refs/heads/main/openapi/ankorstore-main-openapi-original.yml
- filename: ankorstore-astral-openapi-original.yml
  format: yaml
  label: Ankorstore Stock Tracking and Logistics API (ASTRAL)
  slug: ankorstore-stock-tracking-and-logistics-api-astral
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankorstore/refs/heads/main/openapi/ankorstore-astral-openapi-original.yml
- filename: ankorstore-fulfillment-openapi-original.yml
  format: yaml
  label: Ankorstore Fulfillment Service API
  slug: ankorstore-fulfillment-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ankorstore/refs/heads/main/openapi/ankorstore-fulfillment-openapi-original.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ankorstore.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: ankorlocal.com
  spf: false
hosts:
- cert_expires: Oct  7 12:47:10 2026 GMT
  host: www.ankorstore.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- host: www.ankorlocal.com
  https: false
- cert_expires: Oct  7 10:35:00 2026 GMT
  host: www.preprod.ankorstore.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ankorstore Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Ankorstore, probed live across 3 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Ankorstore
provider_slug: ankorstore
slug: ankorstore-domain-security
source_filename: ankorstore-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.ankorstore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 12:47:10 2026 GMT\n  hsts: false\n- host: www.ankorlocal.com\n  https: false\n- host: www.preprod.ankorstore.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 10:35:00 2026 GMT\n  hsts: null\ndomains:\n- domain: ankorstore.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ankorlocal.com\n  dnssec: true\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ankorstore/refs/heads/main/security/ankorstore-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Company
- Retail
- Wholesale
- Marketplace
- E-commerce
- Ordering
- Fulfillment
- Catalog
- Webhooks
- JSON:API
---
