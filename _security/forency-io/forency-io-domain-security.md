---
api_specs:
- filename: forency-io-openapi-generated.yml
  format: yaml
  label: Forency API
  slug: forency-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/forency-io/openapi/_ae-authored/forency-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: forency.io
  spf: true
hosts:
- cert_expires: Jan 17 20:53:52 2027 GMT
  host: forency.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Forency Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Forency, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Forency
provider_slug: forency-io
slug: forency-io-domain-security
source_filename: forency-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: forency.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 17 20:53:52 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: forency.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/forency-io/security/forency-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Technology
- Forensics
- Artificial Intelligence
- Sales
---
