---
api_specs:
- filename: newswhip-openapi.yml
  format: yaml
  label: NewsWhip API
  slug: newswhip-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/openapi/newswhip-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: newswhip.com
  spf: true
  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com include:spf.mandrillapp.com include:mktomail.com include:mg-spf.greenhouse.io ~all
hosts:
- host: newswhip.com
  hsts: false
  hsts_max_age: null
  https: true
- host: api.newswhip.com
  hsts: true
  hsts_include_subdomains: true
  hsts_max_age: 15724800
  https: true
- host: developer.newswhip.com
  hsts: true
  hsts_max_age: 31536000
  https: true
kind: domain-security
layout: security
method: probed
name: Newswhip Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for NewsWhip, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS; 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: NewsWhip
provider_slug: newswhip
slug: newswhip-domain-security
source_filename: newswhip-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nhosts:\n- host: newswhip.com\n  https: true\n  hsts: false\n  hsts_max_age: null\n- host: api.newswhip.com\n  https: true\n  hsts: true\n  hsts_max_age: 15724800\n  hsts_include_subdomains: true\n- host: developer.newswhip.com\n  https: true\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: newswhip.com\n  dnssec: false\n  caa: []\n  spf: true\n  spf_record: v=spf1 include:_spf.google.com include:_spf.salesforce.com include:spf.mandrillapp.com include:mktomail.com\n    include:mg-spf.greenhouse.io ~all\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newswhip/refs/heads/main/security/newswhip-domain-security.yml
summary_line: HSTS · DMARC
tags:
- Company
- Media Intelligence
- Social Media Analytics
- News
- Content Analytics
- Engagement Data
- Predictive Analytics
- Media Monitoring
---
