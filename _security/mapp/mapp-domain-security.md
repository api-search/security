---
api_specs:
- filename: mapp-engage-openapi.yml
  format: yaml
  label: Mapp Engage API
  slug: engage
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/openapi/mapp-engage-openapi.yml
- filename: mapp-intelligence-analytics-openapi.yml
  format: yaml
  label: Mapp Intelligence Analytics API
  slug: intelligence-analytics
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/openapi/mapp-intelligence-analytics-openapi.yml
- filename: mapp-product-catalog-openapi.yml
  format: yaml
  label: Mapp Product Catalog Public API
  slug: product-catalog
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/openapi/mapp-product-catalog-openapi.yml
- filename: mapp-fashion-openapi.yml
  format: yaml
  label: Mapp Fashion API
  slug: fashion
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/openapi/mapp-fashion-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mapp.com
  spf: true
hosts:
- cert_expires: Oct 25 09:50:43 2026 GMT
  host: mapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 19 09:36:10 2026 GMT
  host: docs.mapp.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  4 23:59:59 2026 GMT
  host: api.mapp.com
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Mapp Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mapp Marketing Cloud, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mapp Marketing Cloud
provider_slug: mapp
slug: mapp-domain-security
source_filename: mapp-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 25 09:50:43 2026 GMT\n  hsts: false\n- host: docs.mapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 19 09:36:10 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.mapp.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  4 23:59:59 2026 GMT\n  hsts: false\ndomains:\n- domain: mapp.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mapp/refs/heads/main/security/mapp-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Marketing
- Marketing Automation
- Email
- Analytics
- Customer Data
- Personalization
- Push Notifications
- SMS
- E-Commerce
- Digital Analytics
- Recommendations
---
