---
api_specs:
- filename: spacemesh-v2beta1-openapi-original.json
  format: json
  label: Spacemesh API (v2beta1)
  slug: spacemesh-api-v2beta1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/openapi/spacemesh-v2beta1-openapi-original.json
- filename: spacemesh-v1-openapi-original.json
  format: json
  label: Spacemesh API (v1)
  slug: spacemesh-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/openapi/spacemesh-v1-openapi-original.json
description: ''
domains:
- caa: []
  dmarc: false
  dnssec: false
  domain: spacemesh.io
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: spacemesh.network
  spf: true
hosts:
- host: spacemesh.io
  https: false
- cert_expires: Sep 29 22:02:33 2026 GMT
  host: testnet-api.spacemesh.network
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Spacemesh Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Spacemesh, probed live across 2 host(s) and 2 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC absent.'
provider_name: Spacemesh
provider_slug: spacemesh
slug: spacemesh-domain-security
source_filename: spacemesh-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: spacemesh.io\n  https: false\n- host: testnet-api.spacemesh.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 29 22:02:33 2026 GMT\n  hsts: false\ndomains:\n- domain: spacemesh.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n- domain: spacemesh.network\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacemesh/refs/heads/main/security/spacemesh-domain-security.yml
summary_line: TLSv1.3
tags:
- Company
- Crypto Infrastructure
- Blockchain
- Cryptocurrency
- Proof of Space-Time
- Layer 1
- gRPC
- Node API
- Open Source
---
