---
api_specs:
- filename: stalwart-auth-openapi-generated.yml
  format: yaml
  label: Stalwart Auth overview API
  slug: auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stalwart/openapi/_ae-authored/stalwart-auth-openapi-generated.yml
- filename: stalwart-core-openapi-generated.yml
  format: yaml
  label: Stalwart core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stalwart/openapi/_ae-authored/stalwart-core-openapi-generated.yml
- filename: stalwart-http-openapi-generated.yml
  format: yaml
  label: Stalwart HTTP overview API
  slug: http-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/stalwart/openapi/_ae-authored/stalwart-http-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: stalw.art
  spf: true
hosts:
- cert_expires: Jan 10 21:55:32 2027 GMT
  host: stalw.art
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Stalwart Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Stalwart, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Stalwart
provider_slug: stalwart
slug: stalwart-domain-security
source_filename: stalwart-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: stalw.art\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 10 21:55:32 2027 GMT\n  hsts: false\ndomains:\n- domain: stalw.art\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/stalwart/security/stalwart-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Email
- OpenSource
- Rust
- Collaboration
- Server
- Company
---
