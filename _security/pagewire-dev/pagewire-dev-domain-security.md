---
api_specs:
- filename: pagewire-dev-x402-api-openapi.yml
  format: yaml
  label: pagewire-dev X402 API
  slug: pagewire-dev-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/pagewire-dev/openapi/pagewire-dev-x402-api-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: pagewire.dev
  spf: true
hosts:
- cert_expires: Jan  4 01:27:01 2027 GMT
  host: pagewire.dev
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: pagewire-dev Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for pagewire-dev, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: pagewire-dev
provider_slug: pagewire-dev
slug: pagewire-dev-domain-security
source_filename: pagewire-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: pagewire.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 01:27:01 2027 GMT\n  hsts: false\ndomains:\n- domain: pagewire.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/pagewire-dev/security/pagewire-dev-domain-security.yml
summary_line: TLSv1.3
tags:
- Pay-per-call
- AI Agents
---
