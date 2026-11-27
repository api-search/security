---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: iescrow.io
  spf: true
hosts:
- cert_expires: Feb  6 01:55:13 2027 GMT
  host: iescrow.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: iEscrow Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for iEscrow, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: iEscrow
provider_slug: iescrow-io
slug: iescrow-io-domain-security
source_filename: iescrow-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: iescrow.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Feb  6 01:55:13 2027 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: iescrow.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/iescrow-io/security/iescrow-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Cryptocurrency
- Escrow
- Fintech
- P2P
- Cross-Border
- Services
- Company
---
