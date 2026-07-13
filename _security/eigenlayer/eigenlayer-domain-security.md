---
api_specs:
- filename: eigenlayer-streaming-asyncapi.yml
  format: yaml
  label: EigenDA
  slug: eigenda
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/eigenlayer/refs/heads/main/asyncapi/eigenlayer-streaming-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eigenlayer.xyz
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: eigencloud.xyz
  spf: true
hosts:
- cert_expires: Aug 24 08:27:56 2026 GMT
  host: www.eigenlayer.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 19:07:07 2026 GMT
  host: www.eigencloud.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  2 19:07:07 2026 GMT
  host: docs.eigencloud.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Eigenlayer Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for EigenLayer, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 3 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: EigenLayer
provider_slug: eigenlayer
slug: eigenlayer-domain-security
source_filename: eigenlayer-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.eigenlayer.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 24 08:27:56 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: www.eigencloud.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:07:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.eigencloud.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  2 19:07:07 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: eigenlayer.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: eigencloud.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/eigenlayer/refs/heads/main/security/eigenlayer-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Restaking
- AVS
- Ethereum
- Data Availability
- Verifiable Compute
- Crypto
- Web3
---
