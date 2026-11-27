---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: blockchainanalysis.io
  spf: true
hosts:
- cert_expires: Dec 22 10:14:47 2026 GMT
  host: blockchainanalysis.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BlockchainAnalysis.io Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BlockchainAnalysis.io, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: BlockchainAnalysis.io
provider_slug: blockchainanalysis-io
slug: blockchainanalysis-io-domain-security
source_filename: blockchainanalysis-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: blockchainanalysis.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 22 10:14:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: blockchainanalysis.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/blockchainanalysis-io/security/blockchainanalysis-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Compliance
- Blockchain
- AML
- Transaction Monitoring
---
