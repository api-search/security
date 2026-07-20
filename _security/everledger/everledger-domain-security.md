---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: everledger.io
  spf: true
hosts:
- cert_expires: Oct 15 23:59:59 2026 GMT
  host: everledger.io
  hsts: false
  https: true
  tls_version: TLSv1.3
- cert_expires: Jul 28 06:44:38 2026 GMT
  host: api.everledger.io
  hsts: null
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Everledger Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Everledger, probed live across 2 host(s) and 1 registrable domain(s). 2 host(s) serve HTTPS (up to TLSv1.3); 0 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: Everledger
provider_slug: everledger
slug: everledger-domain-security
source_filename: everledger-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: everledger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct 15 23:59:59 2026 GMT\n  hsts: false\n- host: api.everledger.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jul 28 06:44:38 2026 GMT\n  hsts: null\ndomains:\n- domain: everledger.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/everledger/refs/heads/main/security/everledger-domain-security.yml
summary_line: TLSv1.3 · DMARC
tags:
- Company
- Blockchain
- Provenance
- Supply Chain
- Traceability
- Digital Twin
- Authentication
- Sustainability
- Diamonds
- Luxury Goods
- Anti-Counterfeiting
---
