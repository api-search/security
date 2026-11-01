---
api_specs:
- filename: openapi.yaml
  format: yaml
  label: InsiderFilings API
  slug: insiderfilings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insiderfilings-info/openapi/_original/openapi.yaml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: insiderfilings.info
  spf: true
hosts:
- cert_expires: Jan  4 22:59:47 2027 GMT
  host: insiderfilings.info
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Insiderfilings Info Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for insiderfilings.info, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: insiderfilings.info
provider_slug: insiderfilings-info
slug: insiderfilings-info-domain-security
source_filename: insiderfilings-info-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: insiderfilings.info\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 22:59:47 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: insiderfilings.info\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/insiderfilings-info/security/insiderfilings-info-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Insider Trading
- SEC Filings
- Financial Data
- Research Tools
- Market Data
---
