---
api_specs:
- filename: modernmt-openapi-generated.yml
  format: yaml
  label: ModernMT API
  slug: modernmt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/modernmt/openapi/_ae-authored/modernmt-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: modernmt.com
  spf: true
hosts:
- cert_expires: Nov 29 23:15:19 2026 GMT
  host: www.modernmt.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Modernmt Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for ModernMT, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: ModernMT
provider_slug: modernmt
slug: modernmt-domain-security
source_filename: modernmt-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-27'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.modernmt.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Nov 29 23:15:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: modernmt.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/modernmt/security/modernmt-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- AI
- Translation
- API
- Multilingual
---
