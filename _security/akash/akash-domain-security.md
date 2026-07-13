---
api_specs:
- filename: akash-console-deployment-api.json
  format: json
  label: Akash Console Deployment API
  slug: akash-console-deployment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akash/refs/heads/main/openapi/akash-console-deployment-api.json
- filename: akash-blockchain-rest-api.yaml
  format: yaml
  label: Akash Blockchain REST API
  slug: akash-blockchain-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/akash/refs/heads/main/openapi/akash-blockchain-rest-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: akash.network
  spf: true
- caa: []
  dmarc: false
  dnssec: false
  domain: akashnet.net
  spf: false
hosts:
- cert_expires: Sep  3 18:16:30 2026 GMT
  host: akash.network
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Sep  3 18:16:30 2026 GMT
  host: console-api.akash.network
  hsts: null
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 13:35:28 2026 GMT
  host: api.akashnet.net
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Akash Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Akash Network, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Akash Network
provider_slug: akash
slug: akash-domain-security
source_filename: akash-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: akash.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 18:16:30 2026 GMT\n  hsts: false\n- host: console-api.akash.network\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep  3 18:16:30 2026 GMT\n  hsts: null\n- host: api.akashnet.net\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 13:35:28 2026 GMT\n  hsts: null\ndomains:\n- domain: akash.network\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n- domain: akashnet.net\n  dnssec: false\n  caa: []\n  spf: false\n  dmarc: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/akash/refs/heads/main/security/akash-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cloud Computing
- Decentralized
- Blockchain
- Kubernetes
- GPU
- AI Inference
- Cosmos
- Web3
---
