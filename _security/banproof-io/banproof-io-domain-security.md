---
description: ''
domains:
- caa: []
  dmarc: true
  dmarc_policy: none
  dnssec: true
  domain: banproof.io
  spf: true
hosts:
- cert_expires: Jan  4 02:30:31 2027 GMT
  host: banproof.io
  hsts: true
  hsts_max_age: 63072000
  https: true
  tls_version: TLSv1.3
hosts_probed: 1
kind: domain-security
layout: security
method: probed
name: BanProof AI Domain Security
name_suffix: Domain Security
overview: 'Domain security posture for BanProof AI, probed live across 1 host(s) and 1 registrable domain(s). 1 host(s) serve HTTPS (up to TLSv1.3); 1 advertise HSTS. Email/DNS controls: DNSSEC present, SPF present, DMARC present (p=none).'
provider_name: BanProof AI
provider_slug: banproof-io
slug: banproof-io-domain-security
source_filename: banproof-io-domain-security.yml
source_heading: Domain Security
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: probed\nsource: live DNS/TLS/HTTP probes of apis.yml + OpenAPI hosts\nhosts:\n- host: banproof.io\n  https: true\n  tls_version: TLSv1.3\n  cert_expires: Jan  4 02:30:31 2027 GMT\n  hsts: true\n  hsts_max_age: 63072000\ndomains:\n- domain: banproof.io\n  dnssec: true\n  caa: []\n  spf: true\n  dmarc: true\n  dmarc_policy: none\n"
source_yaml_url: https://artifacts.apis.io/banproof-io/security/banproof-io-domain-security.yml
summary_line: TLSv1.3 · HSTS · DNSSEC · DMARC
tags:
- Compliance
- TikTok
- Amazon
- Affiliates
- Artificial Intelligence
- Video
- ScriptAudit
---
