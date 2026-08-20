---
api_specs:
- filename: moloco-ads-campaign-management-openapi.yml
  format: yaml
  label: Moloco Ads Campaign Management API
  slug: moloco-ads-campaign-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-ads-campaign-management-openapi.yml
- filename: moloco-cloud-auth-openapi.yml
  format: yaml
  label: Moloco Cloud Auth API
  slug: moloco-cloud-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-cloud-auth-openapi.yml
- filename: moloco-commerce-media-management-openapi.yml
  format: yaml
  label: Moloco Commerce Media Management API
  slug: moloco-commerce-media-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-commerce-media-management-openapi.yml
- filename: moloco-commerce-media-decision-openapi.yml
  format: yaml
  label: Moloco Commerce Media Decision API
  slug: moloco-commerce-media-decision-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-commerce-media-decision-openapi.yml
- filename: moloco-commerce-media-event-openapi.yml
  format: yaml
  label: Moloco Commerce Media Event API
  slug: moloco-commerce-media-event-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-commerce-media-event-openapi.yml
- filename: moloco-commerce-media-webhooks-openapi.yml
  format: yaml
  label: Moloco Commerce Media Webhooks
  slug: moloco-commerce-media-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/openapi/moloco-commerce-media-webhooks-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: moloco.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: moloco.cloud
  spf: true
hosts:
- cert_expires: Sep 13 18:26:55 2026 GMT
  host: www.moloco.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 06:35:10 2026 GMT
  host: developer.moloco.cloud
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 23 07:31:30 2026 GMT
  host: api.moloco.cloud
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Moloco Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for MOLOCO, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: MOLOCO
provider_slug: moloco
slug: moloco-domain-security
source_filename: moloco-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.moloco.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 18:26:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developer.moloco.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 06:35:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.moloco.cloud\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 23 07:31:30 2026 GMT\n  hsts: null\ndomains:\n- domain: moloco.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: moloco.cloud\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moloco/refs/heads/main/security/moloco-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Advertising
- AdTech
- Demand-Side Platform
- Retail Media
- Commerce Media
- Programmatic Advertising
- Campaign Management
- Ad Serving
- Machine-Learning
- Mobile Marketing
- Reporting
- user-events
---
