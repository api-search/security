---
api_specs:
- filename: incentivio-mobile-api-openapi.yml
  format: yaml
  label: Incentivio Mobile & Ordering API
  slug: mobile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incentivio/refs/heads/main/openapi/incentivio-mobile-api-openapi.yml
- filename: incentivio-admin-api-openapi.yml
  format: yaml
  label: Incentivio Admin API
  slug: admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/incentivio/refs/heads/main/openapi/incentivio-admin-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: incentivio.com
  spf: true
hosts:
- cert_expires: Sep 15 16:03:36 2026 GMT
  host: incentivio.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 29 12:46:21 2026 GMT
  host: apidocs.incentivio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov 18 23:59:59 2026 GMT
  host: mobile.incentivio.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Incentivio Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Incentivio, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Incentivio
provider_slug: incentivio
slug: incentivio-domain-security
source_filename: incentivio-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: incentivio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 16:03:36 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: apidocs.incentivio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 29 12:46:21 2026 GMT\n  hsts: null\n- host: mobile.incentivio.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 18 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: incentivio.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/incentivio/refs/heads/main/security/incentivio-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Restaurant
- Guest Engagement
- Online Ordering
- Loyalty
- Customer Data Platform
- Marketing Automation
- Analytics
- Reverse ETL
- Restaurant Technology
- Point of Sale
- Gift Cards
- Mobile Ordering
---
