---
api_specs:
- filename: gemfury-gemfury-api-openapi.yml
  format: yaml
  label: Gemfury Developer API
  slug: gemfury-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gemfury/refs/heads/main/openapi/gemfury-gemfury-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: gemfury.com
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: fury.io
  spf: false
hosts:
- cert_expires: Oct  2 23:59:59 2026 GMT
  host: gemfury.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct 30 23:59:59 2026 GMT
  host: api.fury.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Gemfury Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Gemfury, probed live across 2 host(s) and 2 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Gemfury
provider_slug: gemfury
slug: gemfury-domain-security
source_filename: gemfury-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: gemfury.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 23:59:59 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\n- host: api.fury.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 30 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: gemfury.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n- domain: fury.io\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gemfury/refs/heads/main/security/gemfury-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Package Repository
- Private Packages
- Gem
- npm
- PyPI
- Composer
- NuGet
- Go Modules
- Maven
- DEB
- RPM
- Bower
- Rust Crates
- Developer Tools
---
