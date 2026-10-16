---
api_specs:
- filename: apiserpent-openapi-generated.yml
  format: yaml
  label: Contentladder Marketing API
  slug: apiserpent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apiserpent/refs/heads/main/openapi/_ae-authored/apiserpent-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: apiserpent.com
  spf: true
hosts:
- cert_expires: Dec 18 10:13:18 2026 GMT
  host: apiserpent.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Apiserpent Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Contentladder Marketing, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Contentladder Marketing
provider_slug: apiserpent
slug: apiserpent-domain-security
source_filename: apiserpent-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: apiserpent.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 18 10:13:18 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: apiserpent.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apiserpent/refs/heads/main/security/apiserpent-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- SERP
- API
- Search
- Data
---
