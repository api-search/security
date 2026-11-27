---
api_specs:
- filename: fluxapay-xyz-openapi-generated.yml
  format: yaml
  label: FluxA API
  slug: fluxapay-xyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fluxapay-xyz/openapi/_ae-authored/fluxapay-xyz-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: fluxapay.xyz
  spf: true
hosts:
- cert_expires: Feb 15 21:21:40 2027 GMT
  host: fluxapay.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Jan 23 16:24:25 2027 GMT
  host: docs.fluxapay.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Feb  1 01:07:14 2027 GMT
  host: walletapi.fluxapay.xyz
  hsts: null
  https: true
  tls_version: TLSv1.3
hosts_probed: 3
kind: domain-security
layout: security
method: probed
name: FluxA Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FluxA, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: FluxA
provider_slug: fluxapay-xyz
slug: fluxapay-xyz-domain-security
source_filename: fluxapay-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: fluxapay.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb 15 21:21:40 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.fluxapay.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 23 16:24:25 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: walletapi.fluxapay.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  1 01:07:14 2027 GMT\n  hsts: null\ndomains:\n- domain: fluxapay.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/fluxapay-xyz/security/fluxapay-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Payments
- Artificial Intelligence
- Agents
- Infrastructure
---
