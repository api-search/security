---
api_specs:
- filename: synero-ai-api-openapi.json
  format: json
  label: Synero API API
  slug: synero-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/synero-ai/openapi/_original/synero-ai-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: false
  dns_aid:
    checked: '2026-11-25'
    published: false
  dnssec: false
  domain: synero.ai
  spf: false
hosts:
- cert_expires: Feb 11 16:13:41 2027 GMT
  host: synero.ai
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Synero Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Synero, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: Synero
provider_slug: synero-ai
slug: synero-ai-domain-security
source_filename: synero-ai-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: synero.ai\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 11 16:13:41 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: synero.ai\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n  dns_aid:\n    checked: '2026-11-25'\n    published: false\n"
source_yaml_url: https://artifacts.apis.io/synero-ai/security/synero-ai-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
---
