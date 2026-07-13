---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: true
  domain: web3.storage
  spf: true
hosts:
- cert_expires: Sep 15 04:55:36 2026 GMT
  host: web3.storage
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Web3 Storage Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Web3 Storage, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=reject).'
provider_name: Web3 Storage
provider_slug: web3-storage
slug: web3-storage-domain-security
source_filename: web3-storage-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: web3.storage\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Sep 15 04:55:36 2026 GMT\n  hsts: null\ndomains:\n- domain: web3.storage\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/web3-storage/refs/heads/main/security/web3-storage-domain-security.yml
summary_line: TLSv1.3 · DNSSEC · DMARC
tags:
- Cloud Storage And File Sharing
- Public APIs
---
