---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Amobee Campaign API
  slug: amobee-campaign-api
  spec_type: OpenAPI
  url: https://services.amobee.com/campaign/v3/doc/
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: amobee.com
  spf: true
hosts:
- cert_expires: Aug 21 03:48:50 2026 GMT
  host: www.amobee.com
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 16 23:59:59 2026 GMT
  host: services.amobee.com
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Amobee Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Amobee, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Amobee
provider_slug: amobee
slug: amobee-domain-security
source_filename: amobee-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.amobee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 03:48:50 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\n- host: services.amobee.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 16 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: amobee.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amobee/refs/heads/main/security/amobee-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Digital Advertising
- DSP
- Programmatic
- Campaign Management
- Audience Targeting
- Data Management Platform
- Ad Tech
- Samsung Ads
---
