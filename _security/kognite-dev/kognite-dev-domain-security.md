---
api_specs:
- filename: kognite-dev-openapi-generated.yml
  format: yaml
  label: Kognite API
  slug: kognite-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/kognite-dev/openapi/_ae-authored/kognite-dev-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: kognite.dev
  spf: true
hosts:
- cert_expires: Jan 18 22:49:23 2027 GMT
  host: kognite.dev
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Kognite Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Kognite, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Kognite
provider_slug: kognite-dev
slug: kognite-dev-domain-security
source_filename: kognite-dev-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: kognite.dev\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 18 22:49:23 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: kognite.dev\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/kognite-dev/security/kognite-dev-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Artificial Intelligence
- Memory
- Platform
- MCP
---
