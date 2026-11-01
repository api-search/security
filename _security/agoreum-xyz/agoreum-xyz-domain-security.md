---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: quarantine
  dnssec: true
  domain: agoreum.xyz
  spf: true
hosts:
- cert_expires: Dec 17 05:54:55 2026 GMT
  host: agoreum.xyz
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: Agoreum Xyz Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for agoreum-xyz, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=quarantine).'
provider_name: agoreum-xyz
provider_slug: agoreum-xyz
slug: agoreum-xyz-domain-security
source_filename: agoreum-xyz-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: agoreum.xyz\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Dec 17 05:54:55 2026 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: agoreum.xyz\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: quarantine\n"
source_yaml_url: https://artifacts.apis.io/agoreum-xyz/security/agoreum-xyz-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Company
- AI
- Fintech
- Marketplace
- Web3
---
