---
api_specs:
- filename: crossenagage-user-management-v2-openapi.yml
  format: yaml
  label: CrossEngage User Management API v2
  slug: user-management-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/openapi/crossenagage-user-management-v2-openapi.yml
- filename: crossenagage-user-management-v1-openapi.yml
  format: yaml
  label: CrossEngage User Management API v1
  slug: user-management-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/openapi/crossenagage-user-management-v1-openapi.yml
- filename: crossenagage-product-feed-openapi.yml
  format: yaml
  label: CrossEngage Product Feed API
  slug: product-feed
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/openapi/crossenagage-product-feed-openapi.yml
- filename: crossenagage-raw-export-v1-openapi.yml
  format: yaml
  label: CrossEngage Raw Export API
  slug: raw-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/openapi/crossenagage-raw-export-v1-openapi.yml
- filename: crossenagage-statistics-v1-openapi.yml
  format: yaml
  label: CrossEngage Statistics API
  slug: statistics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/openapi/crossenagage-statistics-v1-openapi.yml
- filename: crossenagage-file-attachments-v1-openapi.yml
  format: yaml
  label: CrossEngage File Attachments API
  slug: file-attachments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/openapi/crossenagage-file-attachments-v1-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: crossengage.io
  spf: true
hosts:
- cert_expires: Dec 23 23:59:59 2026 GMT
  host: api.documentation.crossengage.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 30 23:59:59 2026 GMT
  host: api.crossengage.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Crossenagage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for CrossEngage, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: CrossEngage
provider_slug: crossenagage
slug: crossenagage-domain-security
source_filename: crossenagage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: api.documentation.crossengage.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 23:59:59 2026 GMT\n  hsts: false\n- host: api.crossengage.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 30 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: crossengage.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crossenagage/refs/heads/main/security/crossenagage-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Customer Data Platform
- Marketing
- Customer Engagement
- Marketing Automation
- Cross-Channel
- Personalization
- Predictive Analytics
- Segmentation
- Campaign Management
- Product Feed
- Data Export
- Webhook
- Web Tracking
- Germany
---
