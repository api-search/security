---
api_specs:
- filename: klaviyo-openapi.json
  format: json
  label: Klaviyo API
  slug: klaviyo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/klaviyo/refs/heads/main/openapi/klaviyo-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: klaviyo.com
  spf: true
hosts:
- cert_expires: Sep 18 18:43:48 2026 GMT
  host: www.klaviyo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  9 05:58:03 2026 GMT
  host: developers.klaviyo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 18 18:43:48 2026 GMT
  host: a.klaviyo.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Klaviyo Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Klaviyo, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Klaviyo
provider_slug: klaviyo
slug: klaviyo-domain-security
source_filename: klaviyo-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.klaviyo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 18:43:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: developers.klaviyo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  9 05:58:03 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: a.klaviyo.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 18 18:43:48 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: klaviyo.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klaviyo/refs/heads/main/security/klaviyo-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Marketing
- Email
- SMS
- Customer Data
- Ecommerce
- Automation
---
