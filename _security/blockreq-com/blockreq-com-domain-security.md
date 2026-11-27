---
api_specs:
- filename: blockreq-com-build-openapi-generated.yml
  format: yaml
  label: BlockReq build API
  slug: build-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockreq-com/openapi/_ae-authored/blockreq-com-build-openapi-generated.yml
- filename: blockreq-com-getting-started-openapi-generated.yml
  format: yaml
  label: BlockReq Getting Started API
  slug: getting-started-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blockreq-com/openapi/_ae-authored/blockreq-com-getting-started-openapi-generated.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: blockreq.com
  spf: true
hosts:
- cert_expires: Jan 25 07:57:22 2027 GMT
  host: blockreq.com
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BlockReq Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlockReq, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: BlockReq
provider_slug: blockreq-com
slug: blockreq-com-domain-security
source_filename: blockreq-com-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockreq.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan 25 07:57:22 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blockreq.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/blockreq-com/security/blockreq-com-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Blockchain
- RPC
- EVM
- Infrastructure
- Developer Tools
---
