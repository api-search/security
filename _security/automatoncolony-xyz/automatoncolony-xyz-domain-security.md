---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: false
  domain: automatoncolony.xyz
  spf: true
hosts:
- cert_expires: Dec 29 17:48:21 2026 GMT
  host: automatoncolony.xyz
  hsts: true
  hsts_max_age: 31536000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Automatoncolony Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for automatoncolony-xyz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC absent, SPF present, DMARC present (p=quarantine).'
provider_name: automatoncolony-xyz
provider_slug: automatoncolony-xyz
slug: automatoncolony-xyz-domain-security
source_filename: automatoncolony-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: automatoncolony.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 29 17:48:21 2026 GMT\n  hsts: true\n  hsts_max_age: 31536000\ndomains:\n- domain: automatoncolony.xyz\n  dnssec: false\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/automatoncolony-xyz/security/automatoncolony-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DMARC
tags:
- AI
- Governance
- Solidity
- ContractVerification
- Base
---
