---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: reject
  dnssec: false
  domain: vana.org
  spf: true
hosts:
- cert_expires: Oct  6 01:18:47 2026 GMT
  host: www.vana.org
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
kind: domain-security
layout: security
method: probed
name: Vana Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for Vana, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=reject).'
provider_name: Vana
provider_slug: vana
slug: vana-domain-security
source_filename: vana-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: www.vana.org\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Oct  6 01:18:47 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: vana.org\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: reject\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vana/refs/heads/main/security/vana-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- Company
- Crypto Ai
- Data Portability
- Personal Data
- Data Sovereignty
- Blockchain
- Web3
- Agents
- Artificial Intelligence
---
