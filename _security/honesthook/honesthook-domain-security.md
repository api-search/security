---
api_specs:
- filename: honesthook-api-openapi.json
  format: json
  label: HonestHook API API
  slug: honesthook-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/openapi/_original/honesthook-api-openapi.json
description: ''
domains:
- caa:
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  - 0 issue "sectigo.com"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: honesthook.com
  spf: true
hosts:
- cert_expires: Dec  5 15:44:48 2026 GMT
  host: honesthook.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Honesthook Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for HonestHook, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: HonestHook
provider_slug: honesthook
slug: honesthook-domain-security
source_filename: honesthook-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: honesthook.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  5 15:44:48 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: honesthook.com\n  dnssec: false\n  caa:\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  - 0 issue \"sectigo.com\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/honesthook/refs/heads/main/security/honesthook-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- API
- Social Media
- Data Aggregation
- SaaS
---
