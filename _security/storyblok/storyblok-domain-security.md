---
api_specs:
- filename: storyblok-content-delivery-api-v2-openapi.yml
  format: yaml
  label: Storyblok Content Delivery API
  slug: storyblok-content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-content-delivery-api-v2-openapi.yml
- filename: storyblok-management-api-openapi.yml
  format: yaml
  label: Storyblok Management API
  slug: storyblok-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-management-api-openapi.yml
- filename: storyblok-image-service-openapi.yml
  format: yaml
  label: Storyblok Image Service
  slug: storyblok-image-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/openapi/storyblok-image-service-openapi.yml
- filename: storyblok-webhooks-asyncapi.yml
  format: yaml
  label: Storyblok Webhooks
  slug: storyblok-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/asyncapi/storyblok-webhooks-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: storyblok.com
  spf: true
hosts:
- cert_expires: Dec  8 23:59:59 2026 GMT
  host: www.storyblok.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: api.storyblok.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 20 23:59:59 2026 GMT
  host: mapi.storyblok.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Storyblok Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Storyblok, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Storyblok
provider_slug: storyblok
slug: storyblok-domain-security
source_filename: storyblok-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.storyblok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  8 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.storyblok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\n- host: mapi.storyblok.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 20 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: storyblok.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/storyblok/refs/heads/main/security/storyblok-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- CMS
- Content Delivery
- Content Management
- Headless CMS
- Image Optimization
- REST API
- Visual Editor
- Webhooks
---
