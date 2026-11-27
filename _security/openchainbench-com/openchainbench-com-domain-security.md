---
api_specs:
- filename: openchainbench-com-openapi-generated.yml
  format: yaml
  label: OpenChainBench API
  slug: openchainbench-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/openchainbench-com/openapi/_ae-authored/openchainbench-com-openapi-generated.yml
description: ''
domains:
- caa:
  - 0 issuewild "digicert.com; cansignhttpexchanges=yes"
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  dmarc: false
  dnssec: false
  domain: openchainbench.com
  spf: true
hosts:
- cert_expires: Feb  4 17:52:47 2027 GMT
  host: openchainbench.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: OpenChainBench Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for OpenChainBench, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: OpenChainBench
provider_slug: openchainbench-com
slug: openchainbench-com-domain-security
source_filename: openchainbench-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: openchainbench.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  4 17:52:47 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: openchainbench.com\n  dnssec: false\n  caa:\n  - 0 issuewild \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://artifacts.apis.io/openchainbench-com/security/openchainbench-com-domain-security.yml
summary_line: TLSv1.3 · HSTS
tags:
- Company
- Cryptocurrency
- Benchmarking
- Open Source
- Infrastructure
---
