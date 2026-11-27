---
api_specs:
- filename: passtru-openapi-generated.yml
  format: yaml
  label: Passtru API
  slug: passtru-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/passtru/openapi/_ae-authored/passtru-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: passtru.io
  spf: true
hosts:
- cert_expires: Jan 30 00:16:49 2027 GMT
  host: passtru.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 30 00:16:49 2027 GMT
  host: login.passtru.io
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 2
kind: domain-security
layout: security
method: probed
name: Passtru Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Passtru, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Passtru
provider_slug: passtru
slug: passtru-domain-security
source_filename: passtru-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-14'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: passtru.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 00:16:49 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: login.passtru.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 30 00:16:49 2027 GMT\n  hsts: null\ndomains:\n- domain: passtru.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/passtru/security/passtru-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Identity Verification
- Age Verification
- KYC
- Document Verification
- Sanctions Screening
---
