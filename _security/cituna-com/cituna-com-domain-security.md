---
api_specs:
- filename: cituna-com-openapi-generated.yml
  format: yaml
  label: Cituna API
  slug: cituna-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cituna-com/openapi/_ae-authored/cituna-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cituna.com
  spf: true
hosts:
- cert_expires: Dec 22 16:38:33 2026 GMT
  host: cituna.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cituna Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cituna, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cituna
provider_slug: cituna-com
slug: cituna-com-domain-security
source_filename: cituna-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cituna.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 16:38:33 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: cituna.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cituna-com/security/cituna-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Artificial Intelligence
- SEO
- Platform
- Visibility
- Marketing
---
