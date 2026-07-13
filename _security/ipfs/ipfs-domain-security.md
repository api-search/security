---
api_specs:
- filename: ipfs-kubo-rpc-api.json
  format: json
  label: IPFS Kubo RPC API
  slug: ipfs-kubo-rpc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipfs/refs/heads/main/openapi/ipfs-kubo-rpc-api.json
- filename: ipfs-pinning-service-api.yaml
  format: yaml
  label: IPFS Pinning Service API
  slug: ipfs-pinning-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ipfs/refs/heads/main/openapi/ipfs-pinning-service-api.yaml
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: ipfs.tech
  spf: true
- caa:
  - 0 issuewild "letsencrypt.org"
  - 0 issuewild "pki.goog; cansignhttpexchanges=yes"
  - 0 issuewild "ssl.com"
  - 0 issue "comodoca.com"
  - 0 issue "digicert.com; cansignhttpexchanges=yes"
  - 0 issue "letsencrypt.org"
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: ipfs.io
  spf: true
hosts:
- cert_expires: Aug 21 19:09:47 2026 GMT
  host: docs.ipfs.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Oct  5 18:53:19 2026 GMT
  host: specs.ipfs.tech
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Aug 23 20:20:37 2026 GMT
  host: ipfs.io
  hsts: false
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Ipfs Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for IPFS, probed live across 3 host(s) and 2 registrable domain(s). 3 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: IPFS
provider_slug: ipfs
slug: ipfs-domain-security
source_filename: ipfs-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: docs.ipfs.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 21 19:09:47 2026 GMT\n  hsts: false\n- host: specs.ipfs.tech\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  5 18:53:19 2026 GMT\n  hsts: false\n- host: ipfs.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Aug 23 20:20:37 2026 GMT\n  hsts: false\ndomains:\n- domain: ipfs.tech\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n- domain: ipfs.io\n  dnssec: true\n  caa:\n  - 0 issuewild \"letsencrypt.org\"\n  - 0 issuewild \"pki.goog; cansignhttpexchanges=yes\"\n  - 0 issuewild \"ssl.com\"\n  - 0 issue \"comodoca.com\"\n  - 0 issue \"digicert.com; cansignhttpexchanges=yes\"\n  - 0 issue \"letsencrypt.org\"\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ipfs/refs/heads/main/security/ipfs-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- IPFS
- Distributed Storage
- Content-Addressed
- Decentralized
- Peer-to-Peer
- File Storage
- DAG
- Pinning
- Gateway
---
