---
api_specs:
- filename: blockrazor-io-openapi-generated.yml
  format: yaml
  label: BlockRazor API
  slug: blockrazor-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockrazor-io/openapi/_ae-authored/blockrazor-io-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: blockrazor.io
  spf: true
hosts:
- cert_expires: Jan 12 23:59:59 2027 GMT
  host: blockrazor.io
  hsts: false
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BlockRazor Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlockRazor, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: BlockRazor
provider_slug: blockrazor-io
slug: blockrazor-io-domain-security
source_filename: blockrazor-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockrazor.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 12 23:59:59 2027 GMT\n  hsts: false\ndomains:\n- domain: blockrazor.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blockrazor-io/security/blockrazor-io-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Blockchain
- Infrastructure
- Low Latency
- Web3
- Data Streams
- Company
---
