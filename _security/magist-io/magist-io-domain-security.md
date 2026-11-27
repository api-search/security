---
api_specs:
- filename: magist-io-openapi-generated.yml
  format: yaml
  label: Magist API
  slug: magist-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magist-io/openapi/_ae-authored/magist-io-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issue "sectigo.com"
  - 0 issue "letsencrypt.org"
  - 0 issue "pki.goog"
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: magist.io
  spf: true
hosts:
- cert_expires: Dec 26 11:46:10 2026 GMT
  host: magist.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Magist Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Magist, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Magist
provider_slug: magist-io
slug: magist-io-domain-security
source_filename: magist-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: magist.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 26 11:46:10 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: magist.io\n  dnssec: false\n  caa:\n  - 0 issue \"sectigo.com\"\n  - 0 issue \"letsencrypt.org\"\n  - 0 issue \"pki.goog\"\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/magist-io/security/magist-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Legal Tech
- Compliance
- Regulatory
- Software-as-a-Service
- Data
---
