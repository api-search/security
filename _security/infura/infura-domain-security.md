---
api_specs:
- filename: infura-asyncapi.yml
  format: yaml
  label: Infura JSON-RPC API
  slug: json-rpc
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/infura/refs/heads/main/asyncapi/infura-asyncapi.yml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: infura.io
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: metamask.io
  spf: true
hosts:
- cert_expires: Aug 23 18:25:19 2026 GMT
  host: www.infura.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 26 02:02:15 2026 GMT
  host: docs.metamask.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  6 23:59:59 2026 GMT
  host: ipfs.infura.io
  hsts: null
  https: true
  tls_version: TLSv1.2
kind: domain-security
layout: security
method: probed
name: Infura Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Infura, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 2 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Infura
provider_slug: infura
slug: infura-domain-security
source_filename: infura-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.infura.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 18:25:19 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: docs.metamask.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 26 02:02:15 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: ipfs.infura.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Oct  6 23:59:59 2026 GMT\n  hsts: null\ndomains:\n- domain: infura.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: metamask.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infura/refs/heads/main/security/infura-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Web3
- Blockchain
- RPC
- Infrastructure
- MetaMask
- ConsenSys
---
