---
api_specs:
- filename: foliofact-com-openapi.yml
  format: yaml
  label: FolioFact API
  slug: foliofact-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/foliofact-com/openapi/foliofact-com-openapi.yml
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: foliofact.com
  spf: false
hosts:
- cert_expires: Jan  3 18:56:57 2027 GMT
  host: foliofact.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Foliofact Com Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for FolioFact, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF absent, DMARC absent.'
provider_name: FolioFact
provider_slug: foliofact-com
slug: foliofact-com-domain-security
source_filename: foliofact-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: foliofact.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  3 18:56:57 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: foliofact.com\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/foliofact-com/security/foliofact-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Stock Research
- SEC Filings
- Fund Holdings
---
