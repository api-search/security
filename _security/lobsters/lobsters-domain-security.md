---
api_specs:
- filename: openapi.yml
  format: yaml
  label: Lobsters API
  slug: lobsters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lobsters/refs/heads/main/openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: lobste.rs
  spf: true
hosts:
- cert_expires: Aug 31 03:17:12 2026 GMT
  host: lobste.rs
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Lobsters Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Lobsters, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Lobsters
provider_slug: lobsters
slug: lobsters-domain-security
source_filename: lobsters-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: lobste.rs\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 31 03:17:12 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: lobste.rs\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lobsters/refs/heads/main/security/lobsters-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Link Aggregation
- Community
- Technology
- News
- Stories
- Comments
- Tags
---
