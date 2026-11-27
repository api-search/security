---
api_specs:
- filename: verifik-co-api-openapi.json
  format: json
  label: Verifik AI — x402 KYC & Verifik proxy Api API
  slug: verifik-ai-x402-kyc-verifik-proxy-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/verifik-co/openapi/_original/verifik-co-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: verifik.co
  spf: true
hosts:
- cert_expires: Dec 19 20:31:24 2026 GMT
  host: verifik.co
  hsts: true
  hsts_max_age: 300
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Verifik Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Verifik, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Verifik
provider_slug: verifik-co
slug: verifik-co-domain-security
source_filename: verifik-co-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-09'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: verifik.co\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 19 20:31:24 2026 GMT\n  hsts: true\n  hsts_max_age: 300\ndomains:\n- domain: verifik.co\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://artifacts.apis.io/verifik-co/security/verifik-co-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- KYC
- AML
- Facial Recognition
---
