---
api_specs:
- filename: subscan-swagger.yaml
  format: yaml
  label: Subscan API
  slug: subscan-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polkadot/refs/heads/main/openapi/subscan-swagger.yaml
- filename: substrate-api-sidecar-openapi.yaml
  format: yaml
  label: Substrate API Sidecar
  slug: substrate-api-sidecar
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polkadot/refs/heads/main/openapi/substrate-api-sidecar-openapi.yaml
- filename: polkadot-rest-api-openapi.json
  format: json
  label: Polkadot REST API
  slug: polkadot-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/polkadot/refs/heads/main/openapi/polkadot-rest-api-openapi.json
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: polkadot.com
  spf: true
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: subscan.io
  spf: true
hosts:
- cert_expires: Sep 13 02:58:49 2026 GMT
  host: polkadot.com
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 17 00:01:50 2026 GMT
  host: support.subscan.io
  hsts: false
  https: true
  tls_version: TLSv1.2
- cert_expires: Aug 21 06:51:20 2026 GMT
  host: polkadot.api.subscan.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Polkadot Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Polkadot, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Polkadot
provider_slug: polkadot
slug: polkadot-domain-security
source_filename: polkadot-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: polkadot.com\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 13 02:58:49 2026 GMT\n  hsts: false\n- host: support.subscan.io\n  https: true\n  tls_version: TLSv1.2\n  cert_expires: Aug 17 00:01:50 2026 GMT\n  hsts: false\n- host: polkadot.api.subscan.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 06:51:20 2026 GMT\n  hsts: null\ndomains:\n- domain: polkadot.com\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: subscan.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/polkadot/refs/heads/main/security/polkadot-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Blockchain
- Polkadot
- Parachain
- Substrate
- Crypto
- Web3
---
