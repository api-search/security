---
api_specs:
- filename: apiclaw-openapi.json
  format: json
  label: APIClaw
  slug: apiclaw
  spec_type: OpenAPI
  url: https://artifacts.apis.io/apiclaw/openapi/_original/apiclaw-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: apiclaw.biz
  spf: false
hosts:
- cert_expires: Nov 21 17:04:55 2026 GMT
  host: apiclaw.biz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: APIClaw Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for APIClaw, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=quarantine).'
provider_name: APIClaw
provider_slug: apiclaw
slug: apiclaw-domain-security
source_filename: apiclaw-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiclaw.biz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 21 17:04:55 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apiclaw.biz\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/apiclaw/security/apiclaw-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Artificial Intelligence
- LLM
- Software-as-a-Service
- Platform
---
