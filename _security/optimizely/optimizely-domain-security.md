---
api_specs:
- filename: optimizely-web-experimentation-openapi.yml
  format: yaml
  label: Optimizely Web Experimentation REST API
  slug: web-experimentation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-web-experimentation-openapi.yml
- filename: optimizely-feature-experimentation-openapi.yml
  format: yaml
  label: Optimizely Feature Experimentation REST API
  slug: feature-experimentation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-feature-experimentation-openapi.yml
- filename: optimizely-campaign-openapi.yml
  format: yaml
  label: Optimizely Campaign REST API
  slug: campaign
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-campaign-openapi.yml
- filename: optimizely-content-delivery-openapi.yml
  format: yaml
  label: Optimizely Content Delivery API
  slug: content-delivery
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-content-delivery-openapi.yml
- filename: optimizely-content-management-openapi.yml
  format: yaml
  label: Optimizely Content Management API
  slug: content-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-content-management-openapi.yml
- filename: optimizely-graph-openapi.yml
  format: yaml
  label: Optimizely Graph API
  slug: graph
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-graph-openapi.yml
- filename: optimizely-data-platform-openapi.yml
  format: yaml
  label: Optimizely Data Platform REST API
  slug: data-platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-data-platform-openapi.yml
- filename: optimizely-cmp-openapi.yml
  format: yaml
  label: Optimizely CMP Open REST API
  slug: cmp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-cmp-openapi.yml
- filename: optimizely-commerce-service-openapi.yml
  format: yaml
  label: Optimizely Commerce Service API
  slug: commerce-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/openapi/optimizely-commerce-service-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: optimizely.com
  spf: true
hosts:
- cert_expires: Sep 19 22:12:52 2026 GMT
  host: www.optimizely.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  3 18:32:33 2026 GMT
  host: docs.developers.optimizely.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 17 20:01:54 2026 GMT
  host: api.optimizely.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optimizely Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optimizely, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Optimizely
provider_slug: optimizely
slug: optimizely-domain-security
source_filename: optimizely-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.optimizely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 19 22:12:52 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.developers.optimizely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  3 18:32:33 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.optimizely.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 17 20:01:54 2026 GMT\n  hsts: null\ndomains:\n- domain: optimizely.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optimizely/refs/heads/main/security/optimizely-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- A/B Testing
- Content Management
- Customer Data
- E-Commerce
- Experimentation
- Feature Flags
- Marketing
---
