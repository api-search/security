---
api_specs:
- filename: tapfiliate-rest-api-openapi.yml
  format: yaml
  label: Tapfiliate REST API
  slug: tapfiliate-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/openapi/tapfiliate-rest-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: tapfiliate.com
  spf: true
hosts:
- cert_expires: Aug 31 03:06:07 2026 GMT
  host: tapfiliate.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Dec 14 23:59:59 2026 GMT
  host: api.tapfiliate.com
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Tapfiliate Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Tapfiliate, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Tapfiliate
provider_slug: tapfiliate
slug: tapfiliate-domain-security
source_filename: tapfiliate-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: tapfiliate.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 03:06:07 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.tapfiliate.com\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Dec 14 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: tapfiliate.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tapfiliate/refs/heads/main/security/tapfiliate-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Affiliate Marketing
- Affiliate Tracking
- Commission Management
- Conversion Tracking
- Partner Programs
- Referral Programs
- Influencer Marketing
---
