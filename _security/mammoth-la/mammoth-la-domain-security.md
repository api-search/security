---
api_specs:
- filename: mammoth-la-openapi-generated.yml
  format: yaml
  label: Mammoth Media API
  slug: mammoth-la-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mammoth-la/openapi/_ae-authored/mammoth-la-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: mammoth.la
  spf: true
hosts:
- cert_expires: Jan 15 20:34:02 2027 GMT
  host: mammoth.la
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Mammoth La Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Mammoth Media, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Mammoth Media
provider_slug: mammoth-la
slug: mammoth-la-domain-security
source_filename: mammoth-la-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-25'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: mammoth.la\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 15 20:34:02 2027 GMT\n  hsts: null\ndomains:\n- domain: mammoth.la\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/mammoth-la/security/mammoth-la-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Crypto Trading
- Social Trading
- Token Utility
- Community Platform
---
