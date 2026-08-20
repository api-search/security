---
api_specs:
- filename: optimyzee-openapi.yml
  format: yaml
  label: Optimyzee Application API
  slug: optimyzee-application-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/optimyzee/refs/heads/main/openapi/optimyzee-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: optimyzee.com
  spf: true
hosts:
- cert_expires: Oct 14 18:49:35 2026 GMT
  host: optimyzee.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 05:52:55 2026 GMT
  host: www.optimyzee.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 05:52:55 2026 GMT
  host: api.optimyzee.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Optimyzee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Optimyzee, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Optimyzee
provider_slug: optimyzee
slug: optimyzee-domain-security
source_filename: optimyzee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: optimyzee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 14 18:49:35 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.optimyzee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 05:52:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.optimyzee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 05:52:55 2026 GMT\n  hsts: null\ndomains:\n- domain: optimyzee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/optimyzee/refs/heads/main/security/optimyzee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Advertising
- Google Ads
- PPC
- Marketing
- Automation
- Artificial Intelligence
- Software-as-a-Service
- Campaign Management
- Search Advertising
- Yelp Ads
- Meta Ads
- Keyword Research
- Reporting
---
