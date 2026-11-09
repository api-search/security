---
api_specs:
- filename: bizzy-fm-about-api-openapi.yml
  format: yaml
  label: Bizzy About API
  slug: bizzy-fm-about-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bizzy-fm/openapi/bizzy-fm-about-api-openapi.yml
- filename: bizzy-fm-stations-api-openapi.yml
  format: yaml
  label: Bizzy Stations API
  slug: bizzy-fm-stations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bizzy-fm/openapi/bizzy-fm-stations-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: bizzy.fm
  spf: true
hosts:
- cert_expires: Dec  7 01:39:53 2026 GMT
  host: bizzy.fm
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Bizzy Fm Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Bizzy, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Bizzy
provider_slug: bizzy-fm
slug: bizzy-fm-domain-security
source_filename: bizzy-fm-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: bizzy.fm\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec  7 01:39:53 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: bizzy.fm\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/bizzy-fm/security/bizzy-fm-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Radio
- Streaming
- Music
- iOS
- macOS
- Company
---
