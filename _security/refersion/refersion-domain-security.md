---
api_specs:
- filename: refersion-rest-api-openapi.yml
  format: yaml
  label: Refersion REST API
  slug: refersion-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/refersion/refs/heads/main/openapi/refersion-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: refersion.com
  spf: true
- caa: []
  dmarc: false
  dnssec: true
  domain: refersion.dev
  spf: true
hosts:
- cert_expires: Sep 28 12:40:40 2026 GMT
  host: www.refersion.com
  hsts: true
  hsts_max_age: 15552000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 29 21:45:01 2026 GMT
  host: www.refersion.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 22 06:17:21 2026 GMT
  host: api.refersion.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Refersion Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Refersion, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: Refersion
provider_slug: refersion
slug: refersion-domain-security
source_filename: refersion-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.refersion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 28 12:40:40 2026 GMT\n  hsts: true\n  hsts_max_age: 15552000\n- host: www.refersion.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 21:45:01 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.refersion.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 22 06:17:21 2026 GMT\n  hsts: null\ndomains:\n- domain: refersion.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: refersion.dev\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/refersion/refs/heads/main/security/refersion-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Affiliate Marketing
- Influencer Marketing
- E-Commerce
- Referral Tracking
- Commission Management
- Shopify
---
