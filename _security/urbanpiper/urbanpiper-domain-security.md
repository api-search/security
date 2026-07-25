---
api_specs:
- filename: urbanpiper-aggregator-api-openapi.yml
  format: yaml
  label: UrbanPiper Aggregator API
  slug: urbanpiper-aggregator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-aggregator-api-openapi.yml
- filename: urbanpiper-menu-api-openapi.yml
  format: yaml
  label: UrbanPiper Menu API
  slug: urbanpiper-menu-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-menu-api-openapi.yml
- filename: urbanpiper-orders-api-openapi.yml
  format: yaml
  label: UrbanPiper Orders API
  slug: urbanpiper-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-orders-api-openapi.yml
- filename: urbanpiper-stores-api-openapi.yml
  format: yaml
  label: UrbanPiper Stores API
  slug: urbanpiper-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-stores-api-openapi.yml
- filename: urbanpiper-webhooks-api-openapi.yml
  format: yaml
  label: UrbanPiper Webhooks API
  slug: urbanpiper-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/openapi/urbanpiper-webhooks-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: urbanpiper.com
  spf: true
hosts:
- cert_expires: Oct  2 14:22:34 2026 GMT
  host: www.urbanpiper.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 05:13:28 2026 GMT
  host: api-docs.urbanpiper.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 21:45:38 2026 GMT
  host: pos-int.urbanpiper.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Urbanpiper Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for UrbanPiper, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: UrbanPiper
provider_slug: urbanpiper
slug: urbanpiper-domain-security
source_filename: urbanpiper-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.urbanpiper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 14:22:34 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-docs.urbanpiper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 05:13:28 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: pos-int.urbanpiper.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 21:45:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: urbanpiper.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urbanpiper/refs/heads/main/security/urbanpiper-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurants
- Food Delivery
- Ordering
- POS
- Aggregators
- Commerce
---
