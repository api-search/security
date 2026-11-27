---
api_specs:
- filename: layout-link-openapi-generated.yml
  format: yaml
  label: Layout API
  slug: layout-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/layout-link/openapi/_ae-authored/layout-link-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: layout.link
  spf: true
hosts:
- cert_expires: Dec 26 15:20:38 2026 GMT
  host: layout.link
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Layout Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Layout, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Layout
provider_slug: layout-link
slug: layout-link-domain-security
source_filename: layout-link-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-15'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: layout.link\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 15:20:38 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: layout.link\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/layout-link/security/layout-link-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Food
- Ordering
- Restaurant
- Developers
---
