---
api_specs:
- filename: luno-streaming-asyncapi.yml
  format: yaml
  label: Luno API
  slug: luno-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/luno/refs/heads/main/asyncapi/luno-streaming-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: luno.com
  spf: true
hosts:
- cert_expires: Sep 12 00:33:41 2026 GMT
  host: www.luno.com
  hsts: true
  hsts_max_age: 60
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Luno Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Luno, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Luno
provider_slug: luno
slug: luno-domain-security
source_filename: luno-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.luno.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 12 00:33:41 2026 GMT\n  hsts: true\n  hsts_max_age: 60\ndomains:\n- domain: luno.com\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/luno/refs/heads/main/security/luno-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- Cryptocurrency
- Exchange
- Bitcoin
- Ethereum
- Trading
- Fintech
- Wallet
- Blockchain
- Financial Services
---
