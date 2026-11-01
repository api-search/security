---
api_specs:
- filename: zeotap-openapi.yml
  format: yaml
  label: Zeotap Profile API
  slug: zeotap-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zeotap/openapi/zeotap-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: zeotap.com
  spf: true
hosts:
- cert_expires: Jan 13 11:06:55 2027 GMT
  host: zeotap.com
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Zeotap Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Zeotap, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Zeotap
provider_slug: zeotap
slug: zeotap-domain-security
source_filename: zeotap-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: zeotap.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 13 11:06:55 2027 GMT\n  hsts: null\ndomains:\n- domain: zeotap.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/zeotap/security/zeotap-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- AI
- Customer-Data-Platform
- Data-Integration
- Identity-Resolution
---
