---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: provenance.io
  spf: true
hosts:
- cert_expires: Sep 13 17:31:33 2026 GMT
  host: provenance.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 08:53:14 2026 GMT
  host: docs.provenance.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep 13 17:31:33 2026 GMT
  host: api.provenance.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Provenance Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Provenance, probed live across 3 host(s) and 1 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Provenance
provider_slug: provenance
slug: provenance-domain-security
source_filename: provenance-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: provenance.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 17:31:33 2026 GMT\n  hsts: false\n- host: docs.provenance.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 08:53:14 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\n- host: api.provenance.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 17:31:33 2026 GMT\n  hsts: null\ndomains:\n- domain: provenance.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/provenance/refs/heads/main/security/provenance-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Blockchain
- Financial Services
- Tokenization
- Real-World Assets
- Cosmos SDK
- gRPC
- Web3
- DeFi
- Digital Assets
---
