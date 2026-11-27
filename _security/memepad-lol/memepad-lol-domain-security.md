---
api_specs:
- filename: memepad-lol-coins-api-openapi.yml
  format: yaml
  label: memepad Coins API
  slug: memepad-lol-coins-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memepad-lol/openapi/memepad-lol-coins-api-openapi.yml
- filename: memepad-lol-creators-api-openapi.yml
  format: yaml
  label: memepad Creators API
  slug: memepad-lol-creators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memepad-lol/openapi/memepad-lol-creators-api-openapi.yml
- filename: memepad-lol-live-api-openapi.yml
  format: yaml
  label: memepad Live API
  slug: memepad-lol-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memepad-lol/openapi/memepad-lol-live-api-openapi.yml
- filename: memepad-lol-mpad-api-openapi.yml
  format: yaml
  label: memepad Mpad API
  slug: memepad-lol-mpad-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memepad-lol/openapi/memepad-lol-mpad-api-openapi.yml
- filename: memepad-lol-platform-api-openapi.yml
  format: yaml
  label: memepad Platform API
  slug: memepad-lol-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/memepad-lol/openapi/memepad-lol-platform-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: memepad.lol
  spf: false
hosts:
- cert_expires: Jan  7 15:07:07 2027 GMT
  host: memepad.lol
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: memepad Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for memepad, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC present (p=reject).'
provider_name: memepad
provider_slug: memepad-lol
slug: memepad-lol-domain-security
source_filename: memepad-lol-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-18'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: memepad.lol\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  7 15:07:07 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: memepad.lol\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/memepad-lol/security/memepad-lol-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Memecoin
- Launchpad
- Cryptocurrency
- South Korea
- Non-Custodial
---
