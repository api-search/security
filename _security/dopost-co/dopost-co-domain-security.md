---
api_specs:
- filename: dopost-openapi.yml
  format: yaml
  label: dopost Social Media Scheduler API
  slug: dopost-social-media-scheduler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dopost-co/refs/heads/main/openapi/dopost-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: dopost.co
  spf: true
hosts:
- cert_expires: Oct  7 08:04:13 2026 GMT
  host: dopost.co
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Dopost Co Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for dopost, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: dopost
provider_slug: dopost-co
slug: dopost-co-domain-security
source_filename: dopost-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: dopost.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  7 08:04:13 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: dopost.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dopost-co/refs/heads/main/security/dopost-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Social Media
- Scheduling
- Publishing
- Instagram
- Facebook
- TikTok
- Pinterest
- X Twitter
- YouTube
- Content Management
- REST
---
