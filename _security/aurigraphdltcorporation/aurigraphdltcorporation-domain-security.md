---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: false
  domain: aurigraph.io
  spf: true
hosts:
- cert_expires: Dec 11 06:52:35 2026 GMT
  host: www.aurigraph.io
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Aurigraphdltcorporation Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Aurigraphdltcorporation, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=none).'
provider_name: Aurigraphdltcorporation
provider_slug: aurigraphdltcorporation
slug: aurigraphdltcorporation-domain-security
source_filename: aurigraphdltcorporation-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-09-26'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.aurigraph.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 11 06:52:35 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: aurigraph.io\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aurigraphdltcorporation/refs/heads/main/security/aurigraphdltcorporation-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Blockchain
- DLT
- Decentralized
- Enterprise
- Platform
- Company
---
