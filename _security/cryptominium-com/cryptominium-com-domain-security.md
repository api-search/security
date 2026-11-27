---
api_specs:
- filename: cryptominium-com-openapi-generated.yml
  format: yaml
  label: Cryptominium API
  slug: cryptominium-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cryptominium-com/openapi/_ae-authored/cryptominium-com-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: cryptominium.com
  spf: true
hosts:
- cert_expires: Dec 23 18:30:25 2026 GMT
  host: cryptominium.com
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Cryptominium Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Cryptominium, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Cryptominium
provider_slug: cryptominium-com
slug: cryptominium-com-domain-security
source_filename: cryptominium-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: cryptominium.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 23 18:30:25 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: cryptominium.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/cryptominium-com/security/cryptominium-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Market Data
- Analytics
- Guides
- Tools
- Company
---
