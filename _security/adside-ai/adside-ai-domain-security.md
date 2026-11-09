---
api_specs:
- filename: adside-ai-openapi.yaml
  format: yaml
  label: Multi-Source Ads API
  slug: multi-source-ads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/adside-ai/openapi/adside-ai-openapi.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: adside.ai
  spf: true
hosts:
- cert_expires: Jan 23 03:09:41 2027 GMT
  host: adside.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Adside Ai Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Adside, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Adside
provider_slug: adside-ai
slug: adside-ai-domain-security
source_filename: adside-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: adside.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 03:09:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: adside.ai\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/adside-ai/security/adside-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Advertising
- Artificial Intelligence
- Marketing
- Software-as-a-Service
- Automation
---
