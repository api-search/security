---
api_specs:
- filename: aidata-stream-openapi-generated.yml
  format: yaml
  label: aidata-stream API
  slug: aidata-stream-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aidata-stream/openapi/_ae-authored/aidata-stream-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: aidata.stream
  spf: true
hosts:
- cert_expires: Dec 31 15:26:26 2026 GMT
  host: aidata.stream
  hsts: true
  hsts_max_age: 2592000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aidata Stream Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for aidata-stream, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: aidata-stream
provider_slug: aidata-stream
slug: aidata-stream-domain-security
source_filename: aidata-stream-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: aidata.stream\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 31 15:26:26 2026 GMT\n  hsts: true\n  hsts_max_age: 2592000\ndomains:\n- domain: aidata.stream\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/aidata-stream/security/aidata-stream-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- AI
- Analytics
- SEO
- Marketing
- Data
---
