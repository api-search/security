---
api_specs:
- filename: acoustic-content-openapi-original.json
  format: json
  label: Acoustic Content API
  slug: acoustic-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acoustic/refs/heads/main/openapi/acoustic-content-openapi-original.json
- filename: acoustic-campaign-rest-swagger-index.json
  format: json
  label: Acoustic Campaign REST API
  slug: acoustic-campaign-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acoustic/refs/heads/main/openapi/acoustic-campaign-rest-swagger-index.json
- filename: 2sBXqQEHNz
  format: yaml
  label: Acoustic Campaign XML API
  slug: acoustic-campaign-xml-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/1643559/2sBXqQEHNz
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: acoustic.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: goacoustic.com
  spf: true
hosts:
- cert_expires: Sep 16 06:57:03 2026 GMT
  host: www.acoustic.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 20:13:42 2026 GMT
  host: developer.goacoustic.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  1 23:59:59 2026 GMT
  host: api-campaign-us-1.goacoustic.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Acoustic Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Acoustic, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: Acoustic
provider_slug: acoustic
slug: acoustic-domain-security
source_filename: acoustic-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.acoustic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 16 06:57:03 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: developer.goacoustic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 20:13:42 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api-campaign-us-1.goacoustic.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  1 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: acoustic.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: goacoustic.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acoustic/refs/heads/main/security/acoustic-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Martech
- Marketing
- Marketing Automation
- Customer Engagement
- Content Management
- Personalization
- Email
- SMS
- Push Notifications
- Headless CMS
- Digital Asset Management
- Customer Data
- GraphQL
- Consent Management
---
