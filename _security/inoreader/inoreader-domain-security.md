---
api_specs:
- filename: inoreader-openapi-generated.yml
  format: yaml
  label: Inoreader API
  slug: inoreader-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inoreader/refs/heads/main/openapi/_ae-authored/inoreader-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: inoreader.com
  spf: true
hosts:
- cert_expires: Nov  5 09:08:50 2026 GMT
  host: inoreader.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Nov  5 09:08:50 2026 GMT
  host: www.inoreader.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Inoreader Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Inoreader, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Inoreader
provider_slug: inoreader
slug: inoreader-domain-security
source_filename: inoreader-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-22'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: inoreader.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 09:08:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.inoreader.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov  5 09:08:50 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: inoreader.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inoreader/refs/heads/main/security/inoreader-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- RSS
- Content Aggregation
- Productivity
---
